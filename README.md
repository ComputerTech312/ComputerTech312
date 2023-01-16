### Hi there 👋
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=computertech312&theme=github_dark)
<!--
**ComputerTech312/ComputerTech312** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

<?php
// Get user's GitHub repos
$username = "computertech312";
$url = "https://api.github.com/users/".$username."/repos";
$curl = curl_init();
curl_setopt_array($curl, array(
    CURLOPT_URL => $url,
    CURLOPT_RETURNTRANSFER => true,
    CURLOPT_HTTPHEADER => array('User-Agent: Awesome-Octocat-App'),
    CURLOPT_FOLLOWLOCATION => true
));
$result = curl_exec($curl);
curl_close($curl);
$repos = json_decode($result, true);

// Calculate top used languages
$languages = array();
foreach ($repos as $repo) {
    $language = $repo["language"];
    if (!array_key_exists($language, $languages)) {
        $languages[$language] = 1;
    } else {
        $languages[$language]++;
    }
}
arsort($languages);

// Create graph
echo "<div style='width: 100%; height: 300px;'>";
$total_repos = count($repos);
$i = 0;
foreach ($languages as $language => $count) {
    $percentage = round(($count/$total_repos)*100);
    echo "<div style='width: ".$percentage."%; height: 100%; background-color: #".dechex(rand(0x000000, 0xFFFFFF))."; float: left;'>";
    echo "<p style='margin-top: 5px; text-align: center;'>".$language." (".$percentage."%)</p>";
    echo "</div>";
    $i++;
    if ($i >= 5) break;
}
echo "</div>";
?>
