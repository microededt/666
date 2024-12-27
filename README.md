
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>彩蛋管理中心</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background-color: #121212;
            color: #e0e0e0;
            margin: 0;
            padding: 0;
        }
        header {
            background: #333;
            color: #fff;
            padding: 1rem 0;
            text-align: center;
        }
        main {
            margin: 2rem auto;
            max-width: 800px;
            background: #1e1e1e;
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
        }
        section {
            margin-bottom: 2rem;
        }
        h1, h2 {
            color: #76c7c0;
        }
        .hall-of-fame {
            background: #252525;
            padding: 1rem;
            border-radius: 5px;
        }
        .hall-of-fame input {
            padding: 0.5rem;
            margin-right: 0.5rem;
        }
        .hall-of-fame button {
            padding: 0.5rem 1rem;
            background: #76c7c0;
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 3px;
        }
        .hall-of-fame button:hover {
            background: #4f9e94;
        }
        ul {
            padding-left: 1.2rem;
        }
        li {
            margin-bottom: 0.5rem;
        }
        a {
            color: #76c7c0;
        }
        a:hover {
            text-decoration: underline;
        }
        .search-box {
            margin-bottom: 2rem;
            text-align: center;
        }
        .search-box input {
            padding: 0.5rem;
            width: 70%;
            margin-right: 0.5rem;
            border: 1px solid #444;
            border-radius: 4px;
            background: #252525;
            color: #e0e0e0;
        }
        .search-box button {
            padding: 0.5rem 1rem;
            background: #76c7c0;
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 4px;
        }
        .search-box button:hover {
            background: #4f9e94;
        }
    </style>
</head>
<body>
    <header>
        <h1>彩蛋管理中心</h1>
        <nav>
            <a href="#employees">员工名称</a> | 
            <a href="#history">公司历史</a> | 
            <a href="#easter-eggs">游戏中著名彩蛋</a> | 
            <a href="#hall-of-fame">名人堂</a> | 
            <a href="#">主页</a>
        </nav>
    </header>
    <main>
        <div class="search-box">
            <input type="text" id="searchInput" placeholder="搜索内容...">
            <button onclick="searchContent()">搜索</button>
        </div>
        <section id="employees">
            <h2>员工名称</h2>
            <p>microed, yidnid, 里斯·恩德</p>
        </section>
        <section id="history">
            <h2>公司历史</h2>
            <p>彩蛋管理中心（EEMC）是一家总部位于德国的创新型企业，以跨领域的管理和解决方案闻名全球。公司成立于20世纪50年代，起初是作为二战后重建德国经济和科研体系的重要一环。其前身为著名的堡司集团（Fortress Corporation），一个专注于军事技术研发的科研机构。随着战后德国经济从军事导向转向民用领域，堡司集团逐步分化重组，催生了多个新兴企业，EEMC便是其中的杰出代表之一。 EEMC最初的使命是将堡司集团的科研技术应用于资源管理与物流领域，帮助德国重建期间的基础设施和工业快速恢复。由于其对系统化管理和资源优化的独到见解，公司在短短数年内便从区域性企业发展为全国性服务商。 进入21世纪，EEMC进一步拓展了业务领域，逐步涉足智能管理系统、可持续资源利用和供应链优化等高科技行业。如今，公司不仅延续了堡司集团在科研与技术领域的优良传统，还成功将这些技术转化为民用市场的核心竞争力。EEMC的使命是通过创新和管理，将复杂问题简单化，为全球客户提供可持续的解决方案。 作为一个脱胎于历史的企业，EEMC承载了技术创新与社会责任的双重使命，展现了德国企业在转型与重建中的坚韧与智慧。</p>
        </section>
        <section id="easter-eggs">
            <h2>游戏中著名彩蛋</h2>
            <ul>
                <li><a href="https://en.wikipedia.org/wiki/Pac-Man" target="_blank">吃豆人（Pac-Man）隐藏的钥匙</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Doom_(1993_video_game)" target="_blank">毁灭战士的隐藏房间</a></li>
                <li><a href="https://en.wikipedia.org/wiki/The_Legend_of_Zelda" target="_blank">塞尔达传说中的第二任务</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Grand_Theft_Auto_V" target="_blank">GTA V的幽灵彩蛋</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Halo:_Combat_Evolved" target="_blank">光环：战斗进化的特别对话</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Portal_(video_game)" target="_blank">传送门的蛋糕彩蛋</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Elder_Scrolls_V:_Skyrim" target="_blank">上古卷轴5：天际中的巨人和奶酪</a></li>
                <li><a href="https://en.wikipedia.org/wiki/World_of_Warcraft" target="_blank">魔兽世界中的烈酒彩蛋</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Metal_Gear_Solid" target="_blank">合金装备的心灵探戈对决</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Red_Dead_Redemption_2" target="_blank">荒野大镖客2的外星人目击</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Batman:_Arkham_City" target="_blank">蝙蝠侠：阿卡姆之城的秘密房间</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Assassin%27s_Creed" target="_blank">刺客信条的历史人物彩蛋</a></li>
            </ul>
        </section>
        <section id="hall-of-fame" class="hall-of-fame">
            <h2>名人堂</h2>
            <p>请输入您的名字，您将成为彩蛋管理中心名人堂的一员：</p>
            <input type="text" id="nameInput" placeholder="输入名字">
            <button onclick="addName()">提交</button>
            <h3>名人名单：</h3>
            <ul id="nameList"></ul>
        </section>
    </main>
    <script>
        // 从 localStorage 加载名人堂名字
        const nameList = document.getElementById('nameList');
        const storedNames = JSON.parse(localStorage.getItem('hallOfFame')) || [];

        function updateNameList() {
            nameList.innerHTML = '';
            storedNames.forEach(name => {
                const li = document.createElement('li');
                li.textContent = name;
                nameList.appendChild(li);
            });
        }

        function addName() {
            const nameInput = document.getElementById('nameInput');
            const name = nameInput.value.trim();
            if (name && !storedNames.includes(name)) {
                storedNames.push(name);
                localStorage.setItem('hallOfFame', JSON.stringify(storedNames));
                updateNameList();
                nameInput.value = '';
            } else {
                alert('请输入有效名字或该名字已存在！');
            }
        }

     // 初始加载名人堂
        updateNameList();

        // 搜索功能
        function searchContent() {
            const searchTerm = document.getElementById('searchInput').value.toLowerCase();
            const sections = document.querySelectorAll('section');
            sections.forEach(section => {
                section.style.display = 'none';
                if (section.id.toLowerCase().includes(searchTerm) || searchTerm === '') {
                    section.style.display = 'block';
                }
            });
        }
    </script>
</body>
</html>
