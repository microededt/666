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
           <nav>
            <a href="#company-overview">公司介绍</a>
            <a href="#basic-info">基本信息</a>
            <a href="#employee-introductions">员工介绍</a>
            <a href="#easter-eggs">著名彩蛋</a>
            <a href="#hall-of-fame">名人堂</a>
        </nav>
        <section id="company-overview">
    <h1>公司介绍</h1>
    <p>彩蛋管理中心（Easter Egg Management Center, EEMC）是一家总部位于德国的创新型企业，以跨领域的管理和解决方案闻名全球。公司成立于20世纪50年代，起初是作为二战后重建德国经济和科研体系的重要一环。其前身为著名的堡司集团（Fortress Corporation），一个专注于军事技术研发的科研机构。随着战后德国经济从军事导向转向民用领域，堡司集团逐步分化重组，催生了多个新兴企业，EEMC便是其中的杰出代表之一。彩蛋管理中心是一家专注于创意彩蛋设计与管理的机构。我们致力于通过巧妙设计的互动彩蛋，提升产品趣味性，增强用户粘性，为客户打造独一无二的用户体验。无论是游戏、网站还是应用程序，EEMC 都能为您提供量身定制的解决方案。
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
    <p><strong>企业使命（Mission）：</strong>通过隐藏的惊喜点亮每一次探索之旅。</p>
    <p><strong>企业愿景（Vision）：</strong>成为全球领先的彩蛋管理服务提供商，让每个用户发现乐趣的无限可能。</p>
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
    <p><strong>产品与服务类型：</strong>提供创意十足的彩蛋概念设计，包括互动小游戏、隐藏任务和趣味内容。</p>
    <p><strong>核心业务领域：</strong></p>
    <ul>
        <li>支持多平台开发，适用于网页、移动端和游戏应用。
</li>
        <li>将彩蛋无缝融入现有产品中，提高用户体验。</li>
        <li>提供实时数据分析与用户反馈报告，优化彩蛋效果。</li>
    </ul>
    <p><strong>具体服务：</strong></p>
    <ul>
        <li>结合节日或品牌活动设计限时彩蛋，为市场推广助力。</li>
        <li>策划趣味互动，吸引用户参与和分享。</li>
    </ul>
</section>

<section id="target-market">
    <h2>目标市场</h2>
    <p><strong>客户群体：</strong>游戏、电商、教育、品牌营销、广告公司</p>
    <p><strong>行业覆盖：</strong>游戏、零售、教育、广告</p>
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
        <li>吸引多个行业（如游戏、电商、教育等）的客户，尤其是初创企业和中小型企业，帮助他们设计和整合创意彩蛋。</li>
        <li>在短期内完善现有的彩蛋设计和管理工具，增加更多创新的互动功能，提升用户体验。</li>
    </ul>
    <p><strong>长期目标：</strong></p>
    <ul>
        <li>引入AI技术，自动生成个性化的彩蛋，提供更多创新的产品，提升服务效率，减少人工干预。</li>
        <li>在不同地区和市场开设分支机构，提供本地化的服务，帮助不同文化和背景的客户创建符合当地特色的彩蛋体验。</li>
    </ul>
</section>

<section id="faq">
    <h2>常见问题 (FAQ)</h2>
    <ul>
        <li><strong>1. 彩蛋服务适合哪些行业？</strong>
            <p>我们的服务适用于电商、游戏、教育、娱乐等多个领域，任何需要提升用户互动的产品都能从中受益。</p>
        </li>
        <li><strong>2. 如何了解彩蛋的使用效果？</strong>
            <p>我们提供详尽的数据分析报告，包括用户点击率、停留时长和反馈意见，帮助客户评估效果。</p>
        </li>
        <li><strong>3. 彩蛋项目开发需要多长时间？</strong>
            <p>视项目复杂度而定，一般为1至4周。</p>
        </li>
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
     <section id="employee-introductions">
            <h2>员工介绍</h2>
            <article>
                <h3>microed - 首席执行官</h3>
                <img src="employee1.jpg" alt="员工1头像">
                <p>microed是一位经验丰富的企业领导者，擅长资源整合和战略规划。在他的带领下，公司实现了连续5年的盈利增长。</p>
            </article>
            <article>
                <h3>yidnid - 技术总监</h3>
                <p>yidnid负责公司技术研发，致力于打造高效的管理系统和数据分析工具。他的技术团队推出了多项行业领先的解决方案。</p>
            </article>
            <article>
                <h3>里斯·恩德 - 营销总监</h3>
                <p>里斯·恩德在市场营销方面有着独到的见解，通过精准的品牌定位和传播策略，使公司在国际市场上脱颖而出。</p>
            </article>
        </section>
</section>
               <section id="easter-eggs">
            <h2>游戏中著名彩蛋</h2>
            <ul>
                <li><a href="https://en.wikipedia.org/wiki/Pac-Man#Legacy" target="_blank">《吃豆人》的隐藏钥匙关卡</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Doom_(1993_video_game)#Secrets" target="_blank">《毁灭战士》的秘密房间</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Adventure_(1979_video_game)#Legacy" target="_blank">《冒险》的隐藏开发者签名</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Diablo_(video_game)#Development" target="_blank">《暗黑破坏神》的奶牛关</a></li>
                <li><a href="https://en.wikipedia.org/wiki/The_Legend_of_Zelda#Game_design" target="_blank">《塞尔达传说》的隐藏迷宫</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Super_Mario_Bros.#Legacy" target="_blank">《超级马里奥兄弟》的秘密管道</a></li>
                <li><a href="https://en.wikipedia.org/wiki/The_Witcher_3:_Wild_Hunt#Reception" target="_blank">《巫师3》的巨魔彩蛋</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Grand_Theft_Auto_V#Reception" target="_blank">《侠盗猎车手V》的幽灵女郎</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Halo_(franchise)#Critical_reception" target="_blank">《光环》的隐藏音乐彩蛋</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Mortal_Kombat#Legacy" target="_blank">《真人快打》的"Toasty!"彩蛋</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Batman:_Arkham_Series#Reception" target="_blank">《蝙蝠侠：阿卡姆疯人院》的隐藏房间</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Portal_(video_game)#Legacy" target="_blank">《传送门》的蛋糕梗</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Call_of_Duty#Reception" target="_blank">《使命召唤》的僵尸模式秘密</a></li>
                <li><a href="https://en.wikipedia.org/wiki/The_Elder_Scrolls_V:_Skyrim#Legacy" target="_blank">《上古卷轴V》的巨人彩蛋</a></li>
                <li><a href="https://en.wikipedia.org/wiki/Assassin%27s_Creed#Reception" target="_blank">《刺客信条》的宇宙彩蛋</a></li>
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
            <p>欢迎你，在历史之中探寻真相之人。你接下要面对的是一个横跨了一百年的家族的迭起兴衰，当然，我们需要你帮我们拨开历史的迷雾，探清前人所没有发现的真相。如果你成功了，你将获得我们家族遗留下来的宝贵财富。</p>
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
