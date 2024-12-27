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
            <ul>
                <li><a href="#employee-microed">microed</a></li>
                <li><a href="#employee-yidnid">yidnid</a></li>
                <li><a href="#employee-rhysend">里斯·恩德</a></li>
            </ul>
        </section>
       <section id="company-overview">
    <h1>公司介绍</h1>
    <p>彩蛋管理中心（Easter Egg Management Center, EEMC）是一家专注于创新管理解决方案和技术开发的全球性企业。自1981年成立以来，公司始终以优化资源配置和提供卓越价值为核心目标，在全球范围内提供高效的服务。</p>
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
        <section id="employee-microed">
            <h2>员工介绍：microed</h2>
            <p>microed 是彩蛋管理中心的首席技术官（CTO），专注于系统优化和新技术研发。他以敏锐的创新思维和严谨的工作态度闻名。</p>
        </section>
        <section id="employee-yidnid">
            <h2>员工介绍：yidnid</h2>
            <p>yidnid 是彩蛋管理中心的运营主管，擅长团队管理和流程优化。他的领导能力使得多个项目得以高效推进。</p>
        </section>
        <section id="employee-rhysend">
            <h2>员工介绍：里斯·恩德</h2>
            <p>里斯·恩德 是彩蛋管理中心的客户关系经理，以出色的沟通能力和客户服务闻名。他是公司与客户之间的桥梁。</p>
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
