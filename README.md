<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Davide Coon - DevOps Engineer</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-color: #f4f7f9;
            --primary-dark: #1e293b;
            --primary-light: #475569;
            --accent-blue: #0284c7;
            --card-bg: #ffffff;
            --border-color: #e2e8f0;
            --font-main: 'Inter', sans-serif;
        }

        body {
            margin: 0;
            padding: 0;
            background-color: var(--bg-color);
            color: var(--primary-dark);
            font-family: var(--font-main);
            line-height: 1.6;
        }

        h1, h2, h3, h4 {
            margin-top: 0;
            color: var(--primary-dark);
        }

        a {
            color: var(--accent-blue);
            text-decoration: none;
            transition: color 0.2s ease;
        }

        a:hover {
            text-decoration: underline;
        }

        /* Header Styling */
        header {
            text-align: center;
            padding: 40px 20px 20px;
            background-color: var(--card-bg);
            border-bottom: 1px solid var(--border-color);
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 5px;
            font-weight: 700;
        }

        header h2 {
            font-size: 1.25rem;
            color: var(--primary-light);
            font-weight: 400;
        }

        nav {
            margin-top: 20px;
        }

        nav a {
            margin: 0 15px;
            font-weight: 600;
            font-size: 0.95rem;
            color: var(--primary-light);
        }
        
        nav a:hover {
            color: var(--accent-blue);
            text-decoration: none;
        }

        /* Layout */
        .container {
            display: flex;
            max-width: 1100px;
            margin: 40px auto;
            gap: 30px;
            padding: 0 20px;
        }

        .sidebar {
            flex: 1;
            min-width: 280px;
            background: var(--card-bg);
            padding: 30px;
            border: 1px solid var(--border-color);
            border-radius: 8px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
            height: fit-content;
        }

        .main-content {
            flex: 2.5;
            background: var(--card-bg);
            padding: 40px;
            border: 1px solid var(--border-color);
            border-radius: 8px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
        }

        /* Sidebar Elements */
        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            margin: 0 auto 20px;
            display: block;
            border: 3px solid var(--border-color);
        }

        .sidebar-section {
            margin-bottom: 30px;
        }

        .sidebar-section h3 {
            font-size: 1.1rem;
            border-bottom: 2px solid var(--border-color);
            padding-bottom: 8px;
            margin-bottom: 15px;
            text-transform: uppercase;
            font-weight: 700;
            letter-spacing: 0.5px;
            color: var(--primary-light);
        }

        .sidebar-section p {
            font-size: 0.95rem;
            color: var(--primary-light);
        }

        /* Main Content Elements */
        .section-title {
            font-size: 1.5rem;
            border-bottom: 2px solid var(--border-color);
            padding-bottom: 10px;
            margin-bottom: 30px;
            text-transform: uppercase;
            font-weight: 700;
            color: var(--primary-dark);
            letter-spacing: 0.5px;
        }

        .item {
            margin-bottom: 35px;
        }

        .item:last-child {
            margin-bottom: 0;
        }

        .item-header {
            display: flex;
            justify-content: space-between;
            align-items: baseline;
            margin-bottom: 5px;
        }

        .item-header h3 {
            margin-bottom: 0;
            font-size: 1.25rem;
            color: var(--accent-blue);
        }

        .item-meta {
            color: var(--primary-light);
            font-size: 0.9rem;
            font-weight: 600;
        }

        .item-subheader {
            font-weight: 700;
            color: var(--primary-dark);
            margin-bottom: 12px;
            font-size: 1.05rem;
        }

        ul {
            padding-left: 20px;
            color: var(--primary-light);
            margin-top: 0;
        }

        li {
            margin-bottom: 8px;
            font-size: 0.95rem;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
        }

        .skills-grid h4 {
            font-size: 1rem;
            margin-bottom: 10px;
            color: var(--primary-dark);
        }

        .interests-list {
            columns: 2;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .container {
                flex-direction: column;
            }
            .item-header {
                flex-direction: column;
            }
            .item-meta {
                margin-top: 5px;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1>Davide Coon</h1>
        <h2>DevOps Engineer</h2>
        <nav>
            <a href="#experiences">Experiences</a>
            <a href="#education">Education</a>
            <a href="#skills">Skills</a>
            <a href="#interests">Interests</a>
        </nav>
    </header>

    <div class="container">
        <!-- Left Sidebar -->
        <aside class="sidebar">
            <img src="https://www.doyoubuzz.com/var/users/_/2017/7/13/21/1455909/avatar/1430963/avatar_cp_630.jpg" alt="Davide Coon" class="profile-img">
            
            <div class="sidebar-section">
                <h3>Contact</h3>
                <p>San Antonio, TX (78253)<br>United States</p>
                <p>
                    <a href="https://www.linkedin.com/in/davide-coon-3bb48468/" target="_blank">LinkedIn</a><br>
                    <a href="https://github.com/utfans05" target="_blank">GitHub</a>
                </p>
            </div>

            <div class="sidebar-section">
                <h3>Status</h3>
                <p>Employed<br>Open to opportunities</p>
            </div>

            <div class="sidebar-section">
                <h3>About Me</h3>
                <p>I'm a DevOps Engineer who's always looking to advance my skills. I love learning new things and teaching others around me about what I already know. I always want to know the "why and how" rather than just utilize a command / tool blindly so I fully understand the process.</p>
            </div>
        </aside>

        <!-- Right Main Content -->
        <main class="main-content">
            
            <!-- Experiences -->
            <section id="experiences" style="margin-bottom: 50px;">
                <h2 class="section-title">Experiences</h2>
                
                <div class="item">
                    <div class="item-header">
                        <h3>Lead DevOps Engineer</h3>
                        <span class="item-meta">July 2019 - Present</span>
                    </div>
                    <div class="item-subheader">ABC Fitness Solutions</div>
                    <ul>
                        <li>Maintained Kubernetes infrastructure utilizing Amazon EKS ensuring high scalability and maintainability by leveraging multiple node groups, spot instances where appropriate and both cluster and application level autoscaling.</li>
                        <li>Work with development teams to ensure a smooth transition from code to production deployments.</li>
                        <li>Develop process requirements related to product infrastructure.</li>
                        <li>Designed and developed Jenkins Pipelines to build, test, containerize and deploy microservices.</li>
                        <li>Configure and maintain an EKS based Kubernetes infrastructure.</li>
                        <li>Track and prioritize work efforts to ensure work is completed in a timely fashion.</li>
                        <li>Educate and assist other engineers to allow them to maintain current skillsets as well as develop new ones.</li>
                        <li>Managed 250+ microservices on 11 Kubernetes clusters with 5k+ pod across 18 different AWS accounts. (~500K per month of resources)</li>
                        <li>Responsible for over 75k lines of Terraform Code.</li>
                    </ul>
                </div>

                <div class="item">
                    <div class="item-header">
                        <h3>Cloud Virtualization Engineer I</h3>
                        <span class="item-meta">September 2015 - July 2019</span>
                    </div>
                    <div class="item-subheader">Rackspace</div>
                    <ul>
                        <li>Provided customer and team support during night shift hours.</li>
                        <li>Education of co-workers on new technologies and novel uses of existing technologies.</li>
                        <li>Support over 50k+ physical servers and 500k+ virtual instances.</li>
                        <li>Maintain the uptime and availability of a global scale infrastructure with systems numbering in the thousands.</li>
                        <li>Guided co-workers and customers on best practices for configuring scalable, production grade server clusters.</li>
                        <li>Troubleshooting and diagnosis of infrastructure issues working with appropriate teams to attain quick and lasting resolutions.</li>
                        <li>Escalation point within company for in-depth technical issues about all Cloud Products, precluding the ability to Google the answer.</li>
                        <li>Starting to experiment with Kuberneties and Docker as the technology is very interesting to me.</li>
                    </ul>
                </div>

                <div class="item">
                    <div class="item-header">
                        <h3>Linux Administrator I</h3>
                        <span class="item-meta">July 2013 - September 2015</span>
                    </div>
                    <div class="item-subheader">Rackspace | San Antonio, TX</div>
                    <ul>
                        <li>Aid customers in application design and configuration to ensure proper scalability for future needs.</li>
                        <li>Front line contact for all Rackspace Cloud Customers.</li>
                        <li>Act as a point of escalation for team members for more difficult configurations and issues.</li>
                    </ul>
                </div>

                <div class="item">
                    <div class="item-header">
                        <h3>Electronic Systems Security Analyst</h3>
                        <span class="item-meta">January 2004 - May 2013</span>
                    </div>
                    <div class="item-subheader">United States Air Force</div>
                    <ul>
                        <li>Monitoring of US Govt. communications assets to ensure Operational Security and Information Security compliance.</li>
                        <li>Subject Matter Expert for Cyber Operational Risk Assessment mission set.</li>
                    </ul>
                </div>
            </section>

            <!-- Education -->
            <section id="education" style="margin-bottom: 50px;">
                <h2 class="section-title">Education</h2>
                
                <div class="item">
                    <div class="item-header">
                        <h3>Computer Science</h3>
                        <span class="item-meta">Since 2015</span>
                    </div>
                    <div class="item-subheader">Grantham University</div>
                    <p style="color: var(--primary-light); font-size: 0.95rem;">83 Credit Hours completed with 3.3 GPA</p>
                </div>
            </section>

            <!-- Skills -->
            <section id="skills" style="margin-bottom: 50px;">
                <h2 class="section-title">Skills</h2>
                <div class="skills-grid">
                    <div>
                        <h4>Code Control</h4>
                        <ul>
                            <li>Github</li>
                            <li>JIRA</li>
                        </ul>
                    </div>
                    <div>
                        <h4>Programming</h4>
                        <ul>
                            <li>Bash</li>
                            <li>Python</li>
                        </ul>
                    </div>
                    <div>
                        <h4>Virtualization</h4>
                        <ul>
                            <li>Openstack</li>
                            <li>OpenVZ</li>
                            <li>XenServer</li>
                            <li>Docker</li>
                            <li>Kubernetes</li>
                        </ul>
                    </div>
                    <div>
                        <h4>Linux</h4>
                        <ul>
                            <li>Ubuntu/Debian</li>
                            <li>RHEL/CentOS</li>
                            <li>Gentoo</li>
                            <li>NGINX/Apache</li>
                            <li>MySql/MariaDB</li>
                            <li>SQLite</li>
                            <li>Alpine Linux</li>
                        </ul>
                    </div>
                    <div>
                        <h4>Automation</h4>
                        <ul>
                            <li>Terraform/Atlantis</li>
                            <li>Harness</li>
                            <li>Spinnaker</li>
                            <li>Chef</li>
                        </ul>
                    </div>
                </div>
            </section>

            <!-- Interests -->
            <section id="interests">
                <h2 class="section-title">Interests</h2>
                <ul class="interests-list">
                    <li>Fishing</li>
                    <li>Computers</li>
                    <li>Linux</li>
                    <li>Boating</li>
                    <li>Playing Bass Guitar</li>
                </ul>
            </section>

        </main>
    </div>

</body>
</html>