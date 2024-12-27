<!DOCTYPE html>
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
            position: relative;
        }
        #login {
            position: absolute;
            top: 10px;
            right: 10px;
            color: #fff;
        }
        #login input {
            margin: 0 5px;
            padding: 5px;
            background: #252525;
            border: 1px solid #444;
            color: #e0e0e0;
            border-radius: 4px;
        }
        #login button {
            padding: 5px 10px;
            background: #76c7c0;
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 4px;
        }
        #login button:hover {
            background: #4f9e94;
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
        #history-between {
            display: none;
            background: #252525;
            padding: 1.5rem;
            border-radius: 8px;
        }
    </style>
</head>
<body>
    <header>
        <h1>彩蛋管理中心</h1>
        <div id="login">
            <input type="text" id="username" placeholder="用户名">
            <input type="password" id="password" placeholder="密码">
            <button onclick="login()">登录</button>
        </div>
    </header>
    <main>
        <div class="search-box">
            <input type="text" id="searchInput" placeholder="搜索内容...">
            <button onclick="searchContent()">搜索</button>
        </div>
        <section id="company-info">
            <h2>公司基本信息</h2>
            <p>公司名称：彩蛋管理中心（Easter Egg Management Center, EEMC）</p>
            <p>成立时间：1981年</p>
            <p>所在地点：德国莱比锡</p>
            <p>员工人数：约1200名</p>
            <p>办公室面积：总部大楼占地5000平方米，并在全球设有5个分支机构</p>
        </section>
        <section id="easter-eggs">
            <h2>游戏中著名彩蛋</h2>
            <ul>
                <li>《吃豆人》的隐藏钥匙关卡</li>
                <li>《毁灭战士》的秘密房间</li>
                <li>《塞尔达传说》的第二任务</li>
                <li>《GTA V》的幽灵彩蛋</li>
                <li>《光环：战斗进化》的隐藏对话</li>
                <li>《上古卷轴 V：天际》的隐秘巨人洞穴</li>
                <li>《荒野大镖客 2》的外星人目击事件</li>
                <li>《魔兽世界》的彩虹桥</li>
                <li>《超级马里奥》的开发者留言</li>
                <li>《巫师 3》的捉迷藏任务</li>
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
        <section id="history-between">
            <h2>历史之间</h2>
            <p>这是只有登录成功后才会看到的模块。</p>
        </section>
    </main>
    <script>
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

        function login() {
            const username = document.getElementById('username').value;
            const password = document.getElementById('password').value;
            if (username === 'nixin' && password === '20220302') {
                document.getElementById('history-between').style.display = 'block';
                alert('登录成功！历史之间模块已解锁。');
            } else {
                alert('用户名或密码错误！');
            }
        }

        updateNameList();
    </script>
</body>
</html>
