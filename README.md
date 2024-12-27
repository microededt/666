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
            <p>彩蛋管理中心（EEMC）是一家总部位于德国的创新型企业，以跨领域的管理和解决方案闻名全球。其前身为著名的堡司集团，随着战后经济转型，成为智能管理系统和资源利用的领导者。</p>
        </section>
        <section id="easter-eggs">
            <h2>游戏中著名彩蛋</h2>
            <ul>
                <li><a href="https://en.wikipedia.org/wiki/Pac-Man" target="_blank">吃豆人（Pac-Man）隐藏的钥匙</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Doom_(1993_video_game)" target="_blank">毁灭战士的隐藏房间</a></li>
                <li><a href="https://en.wikipedia.org/wiki/The_Legend_of_Zelda" target="_blank">塞尔达传说中的第二任务</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Grand_Theft_Auto_V" target="_blank">GTA V的幽灵彩蛋</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Halo:_Combat_Evolved" target="_blank">光环：战斗进化的特别对话</a></li>
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
