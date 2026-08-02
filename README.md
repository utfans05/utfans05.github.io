<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Davide Coon - DevOps Engineer</title>
    <link href="https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;0,700;1,400&family=Playfair+Display:ital,wght@0,600;0,800;1,600&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-cream: #fcfbf8;
            --crimson: #8a1c1c;
            --sage: #8f9c80;
            --text-dark: #2c2a25;
            --text-light: #5a574f;
            --font-heading: 'Playfair Display', serif;
            --font-body: 'Lora', serif;
        }

        body {
            margin: 0;
            padding: 60px 20px;
            background-color: var(--bg-cream);
            color: var(--text-dark);
            font-family: var(--font-body);
            line-height: 1.7;
            /* Subtle paper texture */
            background-image: url("data:image/svg+xml,%3Csvg width='100' height='100' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.8' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100' height='100' filter='url(%23noise)' opacity='0.03'/%3E%3C/svg%3E");
        }

        .resume-wrapper {
            max-width: 800px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.6);
            padding: 50px 60px;
            border: 1px solid rgba(143, 156, 128, 0.2);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.02);
        }

        h1, h2, h3, h4 {
            font-family: var(--font-heading);
            margin: 0;
            font-weight: 600;
        }

        a {
            color: var(--sage);
            text-decoration: none;
            border-bottom: 1px dotted var(--sage);
            transition: color 0.3s ease, border-color 0.3s ease;
        }

        a:hover {
            color: var(--crimson);
            border-bottom-color: var(--crimson);
        }

        /* Header Section */
        header {
            text-align: center;
            margin-bottom: 40px;
        }

        header img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            border: 2px solid var(--sage);
            margin-bottom: 15px;
        }

        header h1 {
            font-size: 2.8rem;
            color: var(--crimson);
            letter-spacing: 1px;
            margin-bottom: 5px;
        }

        header h2 {
            font-size: 1.2rem;
            color: var(--text-light);
            font-style: italic;
            font-weight: 400;
            margin-bottom: 15px;
        }

        .contact-info {
            font-size: 0.95rem;
            color: var(--text-light);
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .contact-info span {
            display: flex;
            align-items: center;
        }

        .contact-info span::after {
            content: "❦";
            color: var(--sage);
            margin-left: 20px;
            font-size: 0.8rem;
        }

        .contact-info span:last-child::after {
            display: none;
        }

        /* Typography & Layout */
        .section-title {
            font-size: 1.6rem;
            color: var(--crimson);
            text-align: center;
            margin: 40px 0 30px;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 50px;
            height: 1px;
            background-color: var(--sage);
            margin: 10px auto 0;
        }

        .intro-text {
            text-align: center;
            font-size: 1.05rem;
            max-width: 650px;
            margin: 0 auto 40px;
            color: var(--text-dark);
            font-style: italic;
        }

        /* Experience Items */
        .job {
            margin-bottom: 35px;
        }

        .job-header {
            display: flex;
            justify-content: space-between;
            align-items: baseline;
            margin-bottom: 5px;
            border-bottom: 1px solid rgba(143, 156, 128, 0.2);
            padding-bottom: 5px;
        }

        .job-title {
            font-size: 1.3rem;
            color: var(--text-dark);
        }

        .job-date {
            font-size: 0.95rem;
            color: var(--text-light);
            font-style: italic;
        }

        .job-company {
            font-weight: 700;
            color: var(--sage);
            margin-bottom: 10px;
            font-size: 1.05rem;
        }

        ul {
            padding-left: 20px;
            margin-top: 10px;
        }

        li {
            margin-bottom: 8px;
            padding-left: 5px;
        }

        li::marker {
            color: var(--crimson);
            font-size: 0.8em;
        }

        /* Skills & Interests Grid */
        .grid-section {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px 40px;
        }

        .grid-item h4 {
            font-size: 1.1rem;
            color: var(--crimson);
            margin-bottom: 10px;
            border-bottom: 1px dotted var(--sage);
            display: inline-block;
        }

        .grid-item p {
            margin: 0;
            color: var(--text-dark);
            line-height: 1.8;
        }

        .status-box {
            text-align: center;
            margin-top: 50px;
            padding: 20px;
            border: 1px solid var(--sage);
            background: rgba(143, 156, 128, 0.05);
            font-style: italic;
            color: var(--text-light);
        }

        @media (max-width: 600px) {
            .resume-wrapper {
                padding: 30px 20px;
            }
            .job-header {
                flex-direction: column;
            }
            .job-date {
                margin-top: 5px;
            }
            .contact-info span::after {
                display: none;
            }
            .contact-info {
                flex-direction: column;
                gap: 10px;
            }
        }
    </style>
</head>
<body>

    <div class="resume-wrapper">
        <header>
            <img src="https://www.doyoubuzz.com/var/users/_/2017/7/13/21/1455909/avatar/1430963/avatar_cp_630.jpg" alt="Davide Coon">
            <h1>Davide Coon</h1>
            <h2>DevOps Engineer</h2>
            
            <div class="contact-info">
                <span>San Antonio, TX (78253)</span>
                <span><a href="https://www.linkedin.com/in/davide-coon-3bb48468/" target="_blank">LinkedIn</a></span>
                <span><a href="https://github.com/utfans05" target="_blank">GitHub</a></span>
            </div>
        </header>

        <p class="intro-text">
            "I'm a DevOps Engineer who's always looking to advance my skills. I love learning new things and teaching others around me about what I already know. I always want to know the 'why and how' rather than just utilize a command or tool blindly so I fully understand the process."
        </p>

        <section>
            <h3 class="section-title">Professional Experience</h3>
            
            <div class="job">
                <div class="job-header">
                    <div class="job-title">Lead DevOps Engineer</div>
                    <div class="job-date">July 2019 — Present</div>
                </div>
                <div class="job-company">ABC Fitness Solutions</div>
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

            <div class="job">
                <div class="job-header">
                    <div class="job-title">Cloud Virtualization Engineer I</div>
                    <div class="job-date">September 2015 — July 2019</div>
                </div>
                <div class="job-company">Rackspace</div>
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

            <div class="job">
                <div class="job-header">
                    <div class="job-title">Linux Administrator I</div>
                    <div class="job-date">July 2013 — September 2015</div>
                </div>
                <div class="job-company">Rackspace</div>
                <ul>
                    <li>Aid customers in application design and configuration to ensure proper scalability for future needs.</li>
                    <li>Front line contact for all Rackspace Cloud Customers.</li>
                    <li>Act as a point of escalation for team members for more difficult configurations and issues.</li>
                </ul>
            </div>

            <div class="job">
                <div class="job-header">
                    <div class="job-title">Electronic Systems Security Analyst</div>
                    <div class="job-date">January 2004 — May 2013</div>
                </div>
                <div class="job-company">United States Air Force</div>
                <ul>
                    <li>Monitoring of US Govt. communications assets to ensure Operational Security and Information Security compliance.</li>
                    <li>Subject Matter Expert for Cyber Operational Risk Assessment mission set.</li>
                </ul>
            </div>
        </section>

        <section>
            <h3 class="section-title">Education</h3>
            <div class="job">
                <div class="job-header">
                    <div class="job-title">Computer Science</div>
                    <div class="job-date">Since 2015</div>
                </div>
                <div class="job-company">Grantham University</div>
                <p>83 Credit Hours completed with 3.3 GPA</p>
            </div>
        </section>

        <section>
            <h3 class="section-title">Technical Expertise</h3>
            <div class="grid-section">
                <div class="grid-item">
                    <h4>Code Control</h4>
                    <p>Github, JIRA</p>
                </div>
                <div class="grid-item">
                    <h4>Programming</h4>
                    <p>Bash, Python</p>
                </div>
                <div class="grid-item">
                    <h4>Virtualization</h4>
                    <p>Openstack, OpenVZ, XenServer, Docker, Kubernetes</p>
                </div>
                <div class="grid-item">
                    <h4>Linux</h4>
                    <p>Ubuntu/Debian, RHEL/CentOS, Gentoo, NGINX/Apache, MySql/MariaDB, SQLite, Alpine Linux</p>
                </div>
                <div class="grid-item">
                    <h4>Automation</h4>
                    <p>Terraform/Atlantis, Harness, Spinnaker, Chef</p>
                </div>
            </div>
        </section>

        <section>
            <h3 class="section-title">Personal Interests</h3>
            <div class="grid-section">
                <div class="grid-item">
                    <p>Fishing • Computers • Linux • Boating • Playing Bass Guitar</p>
                </div>
            </div>
        </section>
        
        <div class="status-box">
            Currently Employed &bull; Open to opportunities
        </div>

    </div>

</body>
</html>