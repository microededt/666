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
            background-color: #f9f9f9;
            margin: 0;
            padding: 0;
        }
        header {
            background: #0078d7;
            color: #fff;
            padding: 1rem 0;
            text-align: center;
        }
        main {
            margin: 2rem auto;
            max-width: 800px;
            background: #fff;
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        section {
            margin-bottom: 2rem;
        }
        h1, h2 {
            color: #333;
        }
        .hall-of-fame {
            background: #f1f1f1;
            padding: 1rem;
            border-radius: 5px;
        }
        .hall-of-fame input {
            padding: 0.5rem;
            margin-right: 0.5rem;
        }
        .hall-of-fame button {
            padding: 0.5rem 1rem;
            background: #0078d7;
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 3px;
        }
        .hall-of-fame button:hover {
            background: #005fa3;
        }
        ul {
            padding-left: 1.2rem;
        }
        li {
            margin-bottom: 0.5rem;
        }
        a {
            color: #0078d7;
        }
        a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <h1>彩蛋管理中心</h1>
    </header>
    <main>
        <section>
            <h2>员工名称</h2>
            <p>microed,yidnid</p>
        </section>
        <section>
            <h2>公司历史</h2>
            <p>彩蛋管理中心成立于1995年，致力于发现和管理世界上所有的彩蛋内容。</p>
        </section>
        <section>
            <h2>游戏中著名彩蛋</h2>
            <ul>
                <li><a href="https://en.wikipedia.org/wiki/Pac-Man" target="_blank">吃豆人（Pac-Man）隐藏的钥匙</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Doom_(1993_video_game)" target="_blank">毁灭战士的隐藏房间</a></li>
                <li><a href="https://en.wikipedia.org/wiki/The_Legend_of_Zelda" target="_blank">塞尔达传说中的第二任务</a></li>
                <!-- 可以继续添加其他游戏链接，共计100个 -->
            </ul>
        </section>
        <section class="hall-of-fame">
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
    </script>
</body>
</html>
