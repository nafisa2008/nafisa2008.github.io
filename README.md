nm
<!DOCTYPE html>
<html>
<head>
    <title>ApnaSaath</title>

    <style>

    /* Applies basic settings to all elements */
    * {
        box-sizing: border-box;
    }

    /* Main webpage layout using Flexbox */
    body {
        margin: 0;
        font-family: Arial, sans-serif;
        background: #f8f6ef;
        color: #354238;

        display: flex;
        flex-direction: column;
        min-height: 100vh;
    }

    /* Styles the website header */
    header {
        background: linear-gradient(135deg, #456b52, #a5bd98);
        color: white;
        text-align: center;
        padding: 35px;

        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }

    header h1 {
        margin: 0;
        font-size: 38px;
    }

    /* Navigation bar using Flexbox */
    nav {
        background: #243d2c;

        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
    }

    /* Styles navigation links */
    nav a, .dropbtn {
        color: white;
        text-decoration: none;
        padding: 16px 22px;
        display: block;
    }

    /* Hover effect for navigation */
    nav a:hover, .dropbtn:hover {
        background: #456b52;
    }

    /* Dropdown container */
    .dropdown {
        position: relative;
    }

    /* Dropdown menu */
    .dropdown-content {
        display: none;
        position: absolute;
        top: 100%;
        left: 0;
        min-width: 220px;
        background: white;
        z-index: 10;
        box-shadow: 0 5px 15px #243d2c20;
    }

    /* Dropdown links */
    .dropdown-content a {
        color: #354238;
        padding: 12px;
    }

    .dropdown-content a:hover {
        background: #e7efe5;
    }

    /* Displays dropdown on hover */
    .dropdown:hover .dropdown-content {
        display: block;
    }

    /* Main content layout using Flexbox */
    main {
        display: flex;
        flex-direction: column;
        align-items: center;
        flex: 1;
        padding: 10px 0;
    }

    /* Styles all content sections */
    section {
        background: white;
        width: 90%;
        max-width: 1000px;
        margin: 20px 0;
        padding: 30px;
        border-radius: 12px;

        display: flex;
        flex-direction: column;
        gap: 15px;

        box-shadow: 0 4px 15px #35423808;
    }

    section h2 {
        color: #294a34;
    }

    /* Arranges feature cards using Flexbox */
    .cards {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        gap: 20px;
    }

    /* Individual feature cards */
    .card {
        background: #edf3e9;
        padding: 22px;
        border-radius: 10px;
        text-align: center;

        flex: 1 1 220px;
        border: 1px solid #dce7d8;
    }

    /* Feature card headings */
    .card h3 {
        color: #456b52;
    }

    /* Community information boxes */
    .community {
        background: #f1f5ed;
        padding: 18px;
        border-radius: 10px;

        display: flex;
        flex-direction: column;
        gap: 8px;
        border-left: 4px solid #8eaa83;
    }

    .community h3 {
        color: #294a34;
        margin-bottom: 0;
    }

    /* Styles buttons */
    .btn {
        align-self: flex-start;
        background: #456b52;
        color: white;
        text-decoration: none;
        padding: 12px 20px;
        border-radius: 6px;
    }

    .btn:hover {
        background: #294a34;
    }

    /* Footer using Flexbox */
    footer {
        background: #243d2c;
        color: white;
        text-align: center;
        padding: 20px;

        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 8px;
    }

    footer p {
        margin: 0;
    }

    /* Responsive layout for mobile screens */
    @media (max-width: 600px) {

        header h1 {
            font-size: 30px;
        }

        nav a, .dropbtn {
            padding: 13px 14px;
        }

        section {
            padding: 20px;
        }

        .cards {
            flex-direction: column;
        }

        .card {
            flex: 1 1 auto;
        }
    }

    </style>
</head>

<body>

    <!-- Website header -->
    <header id="home">
        <h1>ApnaSaath</h1>
        <p>Help When They Need It. Company When They Want It.</p>
    </header>

    <!-- Navigation bar -->
    <nav>

        <!-- Home link -->
        <a href="#home">Home</a>

        <!-- About link -->
        <a href="#about">About Us</a>

        <!-- Features dropdown -->
        <div class="dropdown">
            <a href="#features" class="dropbtn">Our Services ▼</a>

            <!-- Dropdown options -->
            <div class="dropdown-content">
                <a href="#daily-help">Daily Help</a>
                <a href="#safety">Safety & Care</a>
                <a href="#companionship">Companionship</a>
                <a href="#family">Family Connect</a>
            </div>
        </div>

        <!-- Community link -->
        <a href="#community">Our Community</a>

        <!-- Contact link -->
        <a href="#contact">Contact</a>

    </nav>

    <!-- Main content wrapper -->
    <main>

        <!-- About section -->
        <section id="about">

            <h2>About ApnaSaath</h2>

            <p>
                ApnaSaath is a proposed community-focused platform
                designed to support elderly people with everyday
                assistance, safety, companionship and family connections.
                Our goal is to make independent living easier while
                ensuring that no one feels alone.
            </p>

            <p>
                ApnaSaath brings important support services together
                in one simple place. Elderly people can explore local
                assistance, discover social activities and stay connected
                with their loved ones while maintaining their dignity,
                independence and personal choices.
            </p>

            <p>
                Our philosophy is simple: technology should make life
                easier, create stronger communities and bring people
                closer together.
            </p>

            <a href="#features" class="btn">Explore Our Services</a>

        </section>

        <!-- Features section -->
        <section id="features">

            <h2>Our Services</h2>

            <p>
                Four important ways ApnaSaath aims to make everyday
                life safer, easier and more connected.
            </p>

            <!-- Feature cards arranged with Flexbox -->
            <div class="cards">

                <!-- Daily help -->
                <div class="card" id="daily-help">
                    <h3>Daily Help</h3>
                    <p>
                        Get assistance with grocery shopping, small
                        household tasks, bill payments, online services
                        and everyday errands.
                    </p>
                </div>

                <!-- Safety and care -->
                <div class="card" id="safety">
                    <h3>Safety & Care</h3>
                    <p>
                        Explore daily check-ins and quick access to a
                        trusted emergency contact chosen by the user.
                        Safety and peace of mind come first.
                    </p>
                </div>

                <!-- Companionship -->
                <div class="card" id="companionship">
                    <h3>Companionship</h3>
                    <p>
                        Discover walking partners, hobbies, reading
                        groups, community activities and friendly
                        conversations.
                    </p>
                </div>

                <!-- Family connection -->
                <div class="card" id="family">
                    <h3>Family Connect</h3>
                    <p>
                        Help families stay connected through selected
                        updates and request progress, shared only with
                        the elderly user's permission.
                    </p>
                </div>

            </div>

        </section>

        <!-- Community section -->
        <section id="community">

            <h2>Building a Caring Community</h2>

            <p>
                ApnaSaath believes that everyone deserves support,
                respect and meaningful social connections. Our idea
                brings elderly people, families, local helpers and
                community organisations together.
            </p>

            <!-- Elderly users -->
            <div class="community">
                <h3>Elderly Users</h3>
                <p>
                    Support people who live independently, need
                    occasional assistance or want to participate
                    in social and recreational activities.
                </p>
            </div>

            <!-- Family members -->
            <div class="community">
                <h3>Families & Loved Ones</h3>
                <p>
                    Help relatives stay connected from another city
                    or country through updates that their loved ones
                    choose to share.
                </p>
            </div>

            <!-- Helpers and groups -->
            <div class="community">
                <h3>Helpers & Community Groups</h3>
                <p>
                    Create opportunities for appropriately verified
                    local helpers, volunteers, community groups and
                    service providers to support elderly people.
                </p>
            </div>

        </section>

        <!-- Trust section -->
        <section id="trust">

            <h2>Trust Comes First</h2>

            <p>
                The safety, privacy and dignity of elderly people
                are central to the ApnaSaath idea.
            </p>

            <div class="community">
                <h3>Verified Helpers</h3>
                <p>
                    Helpers should undergo appropriate identity
                    verification before accepting service requests.
                </p>
            </div>

            <div class="community">
                <h3>Privacy by Design</h3>
                <p>
                    Users should decide which family members or
                    trusted people can receive their updates.
                </p>
            </div>

            <div class="community">
                <h3>Independence & Choice</h3>
                <p>
                    ApnaSaath aims to provide support without taking
                    away the freedom to make personal decisions.
                </p>
            </div>

        </section>

        <!-- Contact section -->
        <section id="contact">

            <h2>Contact ApnaSaath</h2>

            <p>
                Have an idea, suggestion or feedback for ApnaSaath?
                We would love to hear your thoughts and ideas for
                building a more caring community.
            </p>

            <p>
                Email: Add your official ApnaSaath email address here.
            </p>

            <p>
                Together, we can create a community where every
                elderly person feels safe, supported and connected.
            </p>

            <a href="mailto:your-email@example.com" class="btn">
                Send Us an Email
            </a>

        </section>

    </main>

    <!-- Website footer -->
    <footer>
        <p>ApnaSaath • Safe. Supported. Connected.</p>
        <p>Help When They Need It. Company When They Want It.</p>
        <p>Independent Startup Project Concept</p>
    </footer>

</body>
</html>
