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
        <section id="company-overview">
    <h1>公司介绍</h1>
    <p>彩蛋管理中心（Easter Egg Management Center, EEMC）是一家总部位于德国的创新型企业，以跨领域的管理和解决方案闻名全球。公司成立于20世纪50年代，起初是作为二战后重建德国经济和科研体系的重要一环。其前身为著名的堡司集团（Fortress Corporation），一个专注于军事技术研发的科研机构。随着战后德国经济从军事导向转向民用领域，堡司集团逐步分化重组，催生了多个新兴企业，EEMC便是其中的杰出代表之一。

EEMC最初的使命是将堡司集团的科研技术应用于资源管理与物流领域，帮助德国重建期间的基础设施和工业快速恢复。由于其对系统化管理和资源优化的独到见解，公司在短短数年内便从区域性企业发展为全国性服务商。

进入21世纪，EEMC进一步拓展了业务领域，逐步涉足智能管理系统、可持续资源利用和供应链优化等高科技行业。如今，公司不仅延续了堡司集团在科研与技术领域的优良传统，还成功将这些技术转化为民用市场的核心竞争力。EEMC的使命是通过创新和管理，将复杂问题简单化，为全球客户提供可持续的解决方案。

作为一个脱胎于历史的企业，EEMC承载了技术创新与社会责任的双重使命，展现了德国企业在转型与重建中的坚韧与智慧。</p>
</section>

<section id="basic-info">
    <h2>公司基本信息</h2>
    <p><strong>公司名称：</strong>彩蛋管理中心（Easter Egg Management Center, EEMC）</p>
    <p><strong>成立时间：</strong>1981年</p>
    <p><strong>所在地点：</strong>德国莱比锡</p>
    <p><strong>公司规模：</strong></p>
    <ul>
        <li><strong>员工人数：</strong>约1200名</li>
        <li><strong>办公室面积：</strong>总部大楼占地5000平方米，并在全球设有5个分支机构</li>
    </ul>
</section>

<section id="mission-vision">
    <h2>公司使命和愿景</h2>
    <p><strong>企业使命（Mission）：</strong>通过创新的管理解决方案和技术，优化全球资源配置，为客户提供卓越的价值。</p>
    <p><strong>企业愿景（Vision）：</strong>成为全球管理与技术解决方案领域的领军者，助力企业和社会实现可持续发展。</p>
</section>

<section id="core-values">
    <h2>核心价值观</h2>
    <ul>
        <li><strong>创新驱动：</strong>推动技术和流程的持续改进。</li>
        <li><strong>诚信经营：</strong>以透明、公正和责任为原则。</li>
        <li><strong>客户至上：</strong>将客户的需求放在首位，为其提供量身定制的解决方案。</li>
    </ul>
</section>

<section id="main-business">
    <h2>主营业务</h2>
    <p><strong>产品与服务类型：</strong>智能管理系统、供应链优化解决方案、数据分析服务</p>
    <p><strong>核心业务领域：</strong></p>
    <ul>
        <li>资源管理与物流</li>
        <li>智能技术开发</li>
        <li>可持续供应链设计</li>
    </ul>
    <p><strong>具体服务：</strong></p>
    <ul>
        <li>提供高效的仓储与物流管理系统</li>
        <li>开发定制化的企业数据分析平台</li>
    </ul>
</section>

<section id="target-market">
    <h2>目标市场</h2>
    <p><strong>客户群体：</strong>跨国企业、中小型企业、政府部门</p>
    <p><strong>行业覆盖：</strong>制造业、零售业、物流运输、能源行业</p>
    <p><strong>区域市场：</strong>欧洲、北美、亚洲</p>
</section>

<section id="achievements">
    <h2>公司成就与荣誉</h2>
    <p><strong>里程碑：</strong></p>
    <ul>
        <li>1990年代推出全球首个智能供应链管理平台</li>
    </ul>
    <p><strong>奖项与认证：</strong></p>
    <ul>
        <li>“欧洲最佳创新企业奖” （2018年）</li>
        <li>ISO 9001 质量管理体系认证</li>
    </ul>
</section>

<section id="future-plans">
    <h2>未来发展计划</h2>
    <p><strong>短期目标：</strong></p>
    <ul>
        <li>推出新一代AI驱动的供应链优化工具</li>
        <li>开拓亚太市场，加强区域服务网络</li>
    </ul>
    <p><strong>长期目标：</strong></p>
    <ul>
        <li>在全球主要市场实现碳中和服务的全覆盖</li>
        <li>成为智能管理系统领域的行业标准制定者</li>
    </ul>
</section>

<section id="contact-info">
    <h2>联系方式</h2>
    <p><strong>官方网站：</strong><a href="https://www.eemc.com" target="_blank">www.eemc.com</a></p>
    <p><strong>联系电话：</strong>+49 30 1234 5678</p>
    <p><strong>邮箱地址：</strong><a href="mailto:info@eemc.com">info@eemc.com</a></p>
    <p><strong>社交媒体：</strong></p>
    <ul>
        <li>LinkedIn: <a href="https://linkedin.com/company/eemc" target="_blank">linkedin.com/company/eemc</a></li>
        <li>Twitter: <a href="https://twitter.com/EEMC_Global" target="_blank">@EEMC_Global</a></li>
    </ul>
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
