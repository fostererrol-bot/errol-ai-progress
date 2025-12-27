<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Errol Foster - AI Mastery Progress Tracker 2025-2026</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --esf-red: #C1272D;
            --esf-lime: #8DC63F;
            --esf-blue: #5B7A9F;
            --esf-gold: #D4A556;
            --esf-dark: #2C2C2C;
            --esf-light: #F5F5F5;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background: linear-gradient(135deg, var(--esf-blue) 0%, var(--esf-red) 100%);
            min-height: 100vh;
            padding: 20px;
            overflow-x: hidden;
            word-wrap: break-word;
            overflow-wrap: break-word;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            width: 100%;
        }

        * {
            word-wrap: break-word;
            overflow-wrap: break-word;
            hyphens: auto;
        }
        
        /* Additional text wrapping for specific elements */
        p, div, span, label, h1, h2, h3, h4, h5, h6, li, td, th, a {
            word-wrap: break-word;
            overflow-wrap: break-word;
            word-break: break-word;
        }
        
        input, textarea, select, button {
            max-width: 100%;
            box-sizing: border-box;
        }
        
        /* Prevent horizontal overflow */
        .header, .panel, .roadmap-quarter, .achievement-item, .milestone-item,
        .daily-reminder, .progress-summary, .quarter-focus, .milestone-content,
        .achievement-description, .milestone-description, .achievement-title, .milestone-title {
            overflow-wrap: break-word;
            word-break: break-word;
            max-width: 100%;
        }

        .header {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            margin-bottom: 30px;
            text-align: center;
            position: relative;
        }

        .conveyor-logo {
            max-width: 250px;
            height: auto;
            margin: 0 auto 25px;
            display: block;
        }

        .header-logo {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 15px;
            margin-bottom: 20px;
        }

        .esf-logo-img {
            max-width: 400px;
            width: 100%;
            height: auto;
        }
        
        .conveyor-logo {
            max-width: 300px;
            width: 100%;
            height: auto;
            margin-bottom: 15px;
        }
        
        @media (max-width: 768px) {
            .esf-logo-img {
                max-width: 300px;
            }
            
            .conveyor-logo {
                max-width: 200px;
            }
        }
        
        @media (max-width: 480px) {
            .esf-logo-img {
                max-width: 250px;
            }
            
            .conveyor-logo {
                max-width: 150px;
            }
        }

        .header h1 {
            color: var(--esf-blue);
            font-size: 2.5em;
            margin-bottom: 5px;
            font-weight: 800;
        }

        .header p {
            color: #666;
            font-size: 1.1em;
            font-weight: 500;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }

        .stat-card {
            background: white;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            text-align: center;
            transition: transform 0.3s;
        }

        .stat-card:hover {
            transform: translateY(-5px);
        }

        .stat-number {
            font-size: 2.5em;
            font-weight: 800;
            color: var(--esf-blue);
            margin-bottom: 10px;
        }

        .stat-label {
            color: #666;
            font-size: 0.9em;
            text-transform: uppercase;
            letter-spacing: 1px;
            font-weight: 600;
        }

        .main-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            margin-bottom: 30px;
        }

        .panel {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            word-wrap: break-word;
            overflow-wrap: break-word;
            overflow-x: hidden;
        }

        .panel h2 {
            color: var(--esf-blue);
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
            font-weight: 700;
            word-wrap: break-word;
            overflow-wrap: break-word;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            color: #333;
            font-weight: 600;
        }

        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            max-width: 100%;
            padding: 12px;
            border: 2px solid #e0e0e0;
            border-radius: 8px;
            font-size: 1em;
            font-family: 'Montserrat', sans-serif;
            transition: border-color 0.3;
            word-wrap: break-word;
            overflow-wrap: break-word;
            box-sizing: border-box;
        }

        .form-group input:focus,
        .form-group textarea:focus,
        .form-group select:focus {
            outline: none;
            border-color: var(--esf-blue);
        }

        .form-group textarea {
            resize: vertical;
            min-height: 100px;
            white-space: pre-wrap;
        }

        .btn {
            background: linear-gradient(135deg, var(--esf-blue) 0%, var(--esf-red) 100%);
            color: white;
            border: none;
            padding: 15px 30px;
            border-radius: 8px;
            font-size: 1em;
            font-weight: 700;
            font-family: 'Montserrat', sans-serif;
            cursor: pointer;
            width: 100%;
            transition: transform 0.2s, box-shadow 0.2s;
        }

        .btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(91, 122, 159, 0.4);
        }

        .achievement-item {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 15px;
            border-left: 4px solid var(--esf-blue);
            transition: transform 0.2s;
            word-wrap: break-word;
            overflow-wrap: break-word;
            overflow-x: hidden;
        }

        .achievement-item:hover {
            transform: translateX(5px);
        }

        .achievement-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 10px;
            flex-wrap: wrap;
            gap: 10px;
        }

        .achievement-type {
            display: inline-block;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.85em;
            font-weight: 600;
            text-transform: uppercase;
        }

        .type-linkedin { background: var(--esf-blue); color: white; }
        .type-project { background: var(--esf-lime); color: white; }
        .type-course { background: var(--esf-red); color: white; }
        .type-milestone { background: var(--esf-gold); color: #333; }

        .achievement-date {
            color: #999;
            font-size: 0.9em;
        }

        .achievement-title {
            font-weight: 600;
            color: #333;
            margin-bottom: 8px;
            font-size: 1.1em;
            word-wrap: break-word;
            overflow-wrap: break-word;
        }

        .achievement-description {
            color: #666;
            line-height: 1.6;
            word-wrap: break-word;
            overflow-wrap: break-word;
            white-space: pre-wrap;
        }

        .achievement-link {
            display: inline-block;
            margin-top: 10px;
            color: var(--esf-blue);
            text-decoration: none;
            font-weight: 600;
            word-wrap: break-word;
            overflow-wrap: break-word;
            max-width: 100%;
        }

        .achievement-link:hover {
            text-decoration: underline;
        }

        .delete-btn {
            background: var(--esf-red);
            color: white;
            border: none;
            padding: 5px 15px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 0.85em;
            font-family: 'Montserrat', sans-serif;
            font-weight: 600;
        }

        .delete-btn:hover {
            background: #a01f24;
        }

        .progress-bar-container {
            background: #e0e0e0;
            border-radius: 10px;
            height: 30px;
            margin-top: 10px;
            overflow: hidden;
        }

        .progress-bar {
            background: linear-gradient(135deg, var(--esf-lime) 0%, var(--esf-blue) 100%);
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: 700;
            transition: width 0.5s;
        }

        .tabs {
            display: flex;
            gap: 10px;
            margin-bottom: 20px;
        }

        .tab {
            padding: 10px 20px;
            background: #f0f0f0;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-weight: 600;
            font-family: 'Montserrat', sans-serif;
            transition: all 0.3s;
        }

        .tab.active {
            background: linear-gradient(135deg, var(--esf-blue) 0%, var(--esf-red) 100%);
            color: white;
        }

        .filter-section {
            display: none;
        }

        .filter-section.active {
            display: block;
        }

        @media (max-width: 768px) {
            body {
                padding: 10px;
            }
            
            .main-content {
                grid-template-columns: 1fr;
            }

            .stats-grid {
                grid-template-columns: 1fr 1fr;
            }

            .header h1 {
                font-size: 1.8em;
                word-wrap: break-word;
                overflow-wrap: break-word;
            }
            
            .nav-tabs {
                flex-direction: column;
            }

            .nav-tab {
                width: 100%;
            }

            .quarter-header {
                flex-direction: column;
                align-items: flex-start;
                gap: 10px;
            }
            
            .quarter-title, .milestone-title, .achievement-title {
                font-size: 1.2em;
                word-wrap: break-word;
                overflow-wrap: break-word;
            }
            
            .milestone-description, .achievement-description, .focus-text {
                font-size: 0.9em;
                word-wrap: break-word;
                overflow-wrap: break-word;
            }
            
            .panel {
                padding: 20px 15px;
            }
            
            /* Ensure all text wraps on mobile */
            p, div, span, label, h1, h2, h3, h4, h5, h6, li {
                word-wrap: break-word !important;
                overflow-wrap: break-word !important;
                word-break: break-word !important;
            }
        }
        
        @media (max-width: 480px) {
            body {
                padding: 5px;
            }
            
            .header h1 {
                font-size: 1.5em;
            }
            
            .stat-number {
                font-size: 2em;
            }
            
            .panel {
                padding: 15px 10px;
            }
            
            .btn {
                padding: 12px 20px;
                font-size: 0.95em;
            }
        }

        .export-btn {
            background: var(--esf-lime);
            margin-top: 10px;
        }

        .export-btn:hover {
            box-shadow: 0 5px 15px rgba(141, 198, 63, 0.4);
        }

        .import-btn {
            background: var(--esf-gold);
            color: #333;
            margin-top: 10px;
        }

        .import-btn:hover {
            box-shadow: 0 5px 15px rgba(212, 165, 86, 0.4);
        }

        /* Navigation */
        .nav-tabs {
            display: flex;
            gap: 15px;
            margin-bottom: 30px;
            background: white;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            flex-wrap: wrap;
        }

        .nav-tab {
            padding: 15px 30px;
            background: #f0f0f0;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            font-weight: 700;
            font-size: 1em;
            font-family: 'Montserrat', sans-serif;
            transition: all 0.3s;
            flex: 1;
            min-width: 150px;
        }

        .nav-tab:hover {
            background: #e0e0e0;
        }

        .nav-tab.active {
            background: linear-gradient(135deg, var(--esf-blue) 0%, var(--esf-red) 100%);
            color: white;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(91, 122, 159, 0.4);
        }

        .page {
            display: none;
        }

        .page.active {
            display: block;
        }

        /* Roadmap Styles */
        .roadmap-quarter {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            margin-bottom: 25px;
        }

        .quarter-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            padding-bottom: 15px;
            border-bottom: 3px solid var(--esf-blue);
        }

        .quarter-title {
            font-size: 1.8em;
            color: var(--esf-blue);
            font-weight: 800;
        }

        .quarter-dates {
            color: #666;
            font-size: 1em;
            font-weight: 600;
        }

        .quarter-focus {
            background: #f8f9fa;
            padding: 15px;
            border-radius: 10px;
            margin-bottom: 20px;
            border-left: 4px solid var(--esf-lime);
        }

        .focus-label {
            font-weight: 700;
            color: var(--esf-lime);
            margin-bottom: 5px;
            text-transform: uppercase;
            font-size: 0.9em;
        }

        .focus-text {
            color: #333;
            font-size: 1.1em;
            font-weight: 600;
        }

        .milestone-list {
            display: grid;
            gap: 15px;
        }

        .milestone-item {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
            display: flex;
            align-items: flex-start;
            gap: 15px;
            transition: all 0.3s;
            cursor: pointer;
            border: 2px solid transparent;
            word-wrap: break-word;
            overflow-wrap: break-word;
            overflow-x: hidden;
        }

        .milestone-item:hover {
            border-color: var(--esf-blue);
            transform: translateX(5px);
        }

        .milestone-item.completed {
            background: #e8f5e9;
            border-color: var(--esf-lime);
        }

        .milestone-checkbox {
            width: 24px;
            height: 24px;
            min-width: 24px;
            cursor: pointer;
            margin-top: 2px;
            flex-shrink: 0;
        }

        .milestone-content {
            flex: 1;
            min-width: 0;
            word-wrap: break-word;
            overflow-wrap: break-word;
        }

        .milestone-title {
            font-weight: 700;
            color: #333;
            margin-bottom: 8px;
            font-size: 1.1em;
            word-wrap: break-word;
            overflow-wrap: break-word;
        }

        .milestone-description {
            color: #666;
            line-height: 1.5;
            font-size: 0.95em;
            word-wrap: break-word;
            overflow-wrap: break-word;
            white-space: pre-wrap;
        }

        .milestone-metric {
            display: inline-block;
            background: var(--esf-blue);
            color: white;
            padding: 5px 12px;
            border-radius: 15px;
            font-size: 0.85em;
            font-weight: 700;
            margin-top: 8px;
        }

        .power-badge {
            display: inline-block;
            padding: 4px 10px;
            border-radius: 12px;
            font-size: 0.8em;
            font-weight: 700;
            margin-right: 8px;
            margin-top: 8px;
        }

        .power-automate { background: var(--esf-red); color: white; }
        .power-build { background: var(--esf-blue); color: white; }
        .power-create { background: var(--esf-lime); color: white; }
        .power-connect { background: var(--esf-gold); color: #333; }

        .daily-reminder {
            background: linear-gradient(135deg, var(--esf-gold) 0%, var(--esf-lime) 100%);
            padding: 25px;
            border-radius: 15px;
            margin-bottom: 25px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .daily-reminder h3 {
            color: #333;
            margin-bottom: 15px;
            font-size: 1.5em;
            font-weight: 800;
        }

        .daily-tasks {
            display: grid;
            gap: 10px;
        }

        .daily-task {
            background: white;
            padding: 15px;
            border-radius: 8px;
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .daily-task input[type="checkbox"] {
            width: 20px;
            height: 20px;
            cursor: pointer;
        }

        .daily-task label {
            flex: 1;
            cursor: pointer;
            color: #333;
            font-weight: 600;
        }

        .progress-summary {
            background: white;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            margin-bottom: 25px;
        }

        .progress-summary h3 {
            font-weight: 800;
        }

        .progress-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
            border-bottom: 1px solid #e0e0e0;
        }

        .progress-item:last-child {
            border-bottom: none;
        }

        .progress-label {
            font-weight: 600;
            color: #333;
        }

        .progress-value {
            font-size: 1.2em;
            font-weight: 800;
            color: var(--esf-blue);
        }

        @media (max-width: 768px) {
            .nav-tabs {
                flex-direction: column;
            }

            .nav-tab {
                width: 100%;
            }

            .quarter-header {
                flex-direction: column;
                align-items: flex-start;
                gap: 10px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header -->
        <div class="header">
            <h1>AI Mastery Progress Tracker</h1>
            <p>Errol Foster's Journey to AI Expert 2025-2026</p>
        </div>

        <!-- Navigation Tabs -->
        <div class="nav-tabs">
            <button class="nav-tab active" onclick="switchPage('dashboard')">Dashboard</button>
            <button class="nav-tab" onclick="switchPage('roadmap')">Roadmap</button>
            <button class="nav-tab" onclick="switchPage('achievements')">Achievements</button>
        </div>

        <!-- Dashboard Page -->
        <div id="dashboardPage" class="page active">
            <!-- Stats Grid -->
            <div class="stats-grid">
            <div class="stat-card">
                <div class="stat-number" id="totalAchievements">3</div>
                <div class="stat-label">Total Achievements</div>
            </div>
            <div class="stat-card">
                <div class="stat-number" id="linkedinPosts">1</div>
                <div class="stat-label">LinkedIn Posts</div>
            </div>
            <div class="stat-card">
                <div class="stat-number" id="projectsBuilt">2</div>
                <div class="stat-label">Projects Built</div>
            </div>
            <div class="stat-card">
                <div class="stat-number" id="courseProgress">5%</div>
                <div class="stat-label">Course Progress</div>
            </div>
        </div>

        <!-- Course Progress Bar -->
        <div class="panel" style="margin-bottom: 30px;">
            <h2>AAA Accelerator Course Progress</h2>
            <p style="color: #666; margin-bottom: 15px;">Current: Lesson 1.3 - Field Work (Foundation Section)</p>
            <div class="progress-bar-container">
                <div class="progress-bar" id="courseProgressBar" style="width: 5%;">5%</div>
            </div>
            <button class="btn" style="margin-top: 15px;" onclick="updateCourseProgress()">Update Course Progress</button>
        </div>

        <!-- Main Content -->
        <div class="main-content">
            <!-- Add Achievement Panel -->
            <div class="panel">
                <h2>➕ Add New Achievement</h2>
                <form id="achievementForm">
                    <div class="form-group">
                        <label for="achievementType">Type</label>
                        <select id="achievementType" required>
                            <option value="">Select Type...</option>
                            <option value="linkedin">LinkedIn Post</option>
                            <option value="project">Project Built</option>
                            <option value="course">Course Progress</option>
                            <option value="milestone">Milestone</option>
                        </select>
                    </div>

                    <div class="form-group">
                        <label for="achievementTitle">Title</label>
                        <input type="text" id="achievementTitle" placeholder="e.g., Created Conveyor Automation Tool" required>
                    </div>

                    <div class="form-group">
                        <label for="achievementDescription">Description</label>
                        <textarea id="achievementDescription" placeholder="Add details about your achievement..." required></textarea>
                    </div>

                    <div class="form-group">
                        <label for="achievementLink">Link (Optional)</label>
                        <input type="url" id="achievementLink" placeholder="https://linkedin.com/posts/...">
                    </div>

                    <div class="form-group">
                        <label for="achievementDate">Date</label>
                        <input type="date" id="achievementDate" required>
                    </div>

                    <button type="submit" class="btn">Add Achievement</button>
                </form>

                <button class="btn export-btn" onclick="exportData()">📥 Export Data</button>
                <button class="btn import-btn" onclick="document.getElementById('importFile').click()">📤 Import Data</button>
                <input type="file" id="importFile" accept=".json" style="display: none;" onchange="importData(event)">
            </div>

            <!-- Achievements List Panel -->
            <div class="panel">
                <h2>🏆 Your Achievements</h2>
                
                <!-- Filter Tabs -->
                <div class="tabs">
                    <button class="tab active" onclick="filterAchievements('all')">All</button>
                    <button class="tab" onclick="filterAchievements('linkedin')">LinkedIn</button>
                    <button class="tab" onclick="filterAchievements('project')">Projects</button>
                    <button class="tab" onclick="filterAchievements('course')">Course</button>
                    <button class="tab" onclick="filterAchievements('milestone')">Milestones</button>
                </div>

                <div id="achievementsList"></div>
            </div>
        </div>
        </div>
        <!-- End Dashboard Page -->

        <!-- Roadmap Page -->
        <div id="roadmapPage" class="page">
            <!-- Daily Reminder -->
            <div class="daily-reminder">
                <h3>Today's Focus - <span id="todayDate"></span></h3>
                <div class="daily-tasks" id="dailyTasks">
                    <div class="daily-task">
                        <input type="checkbox" id="task1" onchange="saveDailyProgress()">
                        <label for="task1">Review and respond to comments on latest LinkedIn post</label>
                    </div>
                    <div class="daily-task">
                        <input type="checkbox" id="task2" onchange="saveDailyProgress()">
                        <label for="task2">Complete 30 minutes of AAA Accelerator coursework</label>
                    </div>
                    <div class="daily-task">
                        <input type="checkbox" id="task3" onchange="saveDailyProgress()">
                        <label for="task3">Work on current project/app for 1 hour</label>
                    </div>
                    <div class="daily-task">
                        <input type="checkbox" id="task4" onchange="saveDailyProgress()">
                        <label for="task4">Practice prompt engineering (15 minutes)</label>
                    </div>
                    <div class="daily-task">
                        <input type="checkbox" id="task5" onchange="saveDailyProgress()">
                        <label for="task5">Create or curate content for tomorrow's post</label>
                    </div>
                </div>
            </div>

            <!-- Progress Summary -->
            <div class="progress-summary">
                <h3 style="margin-bottom: 20px;">Overall Progress Summary</h3>
                <div class="progress-item">
                    <span class="progress-label">Q1 Milestones Completed</span>
                    <span class="progress-value" id="q1Progress">0/8</span>
                </div>
                <div class="progress-item">
                    <span class="progress-label">Q2 Milestones Completed</span>
                    <span class="progress-value" id="q2Progress">0/9</span>
                </div>
                <div class="progress-item">
                    <span class="progress-label">Q3 Milestones Completed</span>
                    <span class="progress-value" id="q3Progress">0/8</span>
                </div>
                <div class="progress-item">
                    <span class="progress-label">Q4 Milestones Completed</span>
                    <span class="progress-value" id="q4Progress">0/8</span>
                </div>
                <div class="progress-item">
                    <span class="progress-label">Total Progress</span>
                    <span class="progress-value" id="totalProgress">0%</span>
                </div>
            </div>

            <!-- Q1 2025 -->
            <div class="roadmap-quarter">
                <div class="quarter-header">
                    <div class="quarter-title">Q1 2025</div>
                    <div class="quarter-dates">January - March 2025</div>
                </div>
                <div class="quarter-focus">
                    <div class="focus-label">Focus</div>
                    <div class="focus-text">Foundation + Automate - Build your base and reclaim time</div>
                </div>
                <div class="milestone-list">
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q1-1')">
                        <input type="checkbox" class="milestone-checkbox" id="q1-1" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q1-1')">
                        <div class="milestone-content">
                            <div class="milestone-title">Complete AAA Accelerator Foundation Section</div>
                            <div class="milestone-description">Finish all foundation modules and exercises</div>
                            <span class="power-badge power-build">Build</span>
                            <span class="milestone-metric">Course Module</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q1-2')">
                        <input type="checkbox" class="milestone-checkbox" id="q1-2" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q1-2')">
                        <div class="milestone-content">
                            <div class="milestone-title">Audit All Repetitive Tasks</div>
                            <div class="milestone-description">Create comprehensive list of tasks to automate in 3D design, admin, and content workflows</div>
                            <span class="power-badge power-automate">Automate</span>
                            <span class="milestone-metric">Time Audit</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q1-3')">
                        <input type="checkbox" class="milestone-checkbox" id="q1-3" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q1-3')">
                        <div class="milestone-content">
                            <div class="milestone-title">Set Up 3 Core Automation Workflows</div>
                            <div class="milestone-description">Automate email responses, social media scheduling, and project documentation</div>
                            <span class="power-badge power-automate">Automate</span>
                            <span class="milestone-metric">Save 10+ hrs/week</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q1-4')">
                        <input type="checkbox" class="milestone-checkbox" id="q1-4" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q1-4')">
                        <div class="milestone-content">
                            <div class="milestone-title">Master ChatGPT Custom Instructions</div>
                            <div class="milestone-description">Create tailored prompt templates for design work, client communication, and content creation</div>
                            <span class="power-badge power-connect">Connect</span>
                            <span class="milestone-metric">Prompt Library</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q1-5')">
                        <input type="checkbox" class="milestone-checkbox" id="q1-5" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q1-5')">
                        <div class="milestone-content">
                            <div class="milestone-title">Post on LinkedIn 3x per Week</div>
                            <div class="milestone-description">Build consistent posting habit sharing AI + engineering insights</div>
                            <span class="power-badge power-connect">Connect</span>
                            <span class="milestone-metric">36+ posts</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q1-6')">
                        <input type="checkbox" class="milestone-checkbox" id="q1-6" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q1-6')">
                        <div class="milestone-content">
                            <div class="milestone-title">Build 3 Practice Apps in Replit</div>
                            <div class="milestone-description">Portfolio site, calculator tool, and simple project management system</div>
                            <span class="power-badge power-build">Build</span>
                            <span class="milestone-metric">3 Apps</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q1-7')">
                        <input type="checkbox" class="milestone-checkbox" id="q1-7" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q1-7')">
                        <div class="milestone-content">
                            <div class="milestone-title">Experiment with AI Image Tools</div>
                            <div class="milestone-description">Test Midjourney, DALL-E, and Stable Diffusion for design concepts</div>
                            <span class="power-badge power-create">Create</span>
                            <span class="milestone-metric">3 Tools Tested</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q1-8')">
                        <input type="checkbox" class="milestone-checkbox" id="q1-8" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q1-8')">
                        <div class="milestone-content">
                            <div class="milestone-title">Reach 500 LinkedIn Followers</div>
                            <div class="milestone-description">Grow audience through consistent, valuable content</div>
                            <span class="power-badge power-connect">Connect</span>
                            <span class="milestone-metric">500 followers</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Q2 2025 -->
            <div class="roadmap-quarter">
                <div class="quarter-header">
                    <div class="quarter-title">Q2 2025</div>
                    <div class="quarter-dates">April - June 2025</div>
                </div>
                <div class="quarter-focus">
                    <div class="focus-label">Focus</div>
                    <div class="focus-text">Build + Create - Launch products and scale content</div>
                </div>
                <div class="milestone-list">
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q2-1')">
                        <input type="checkbox" class="milestone-checkbox" id="q2-1" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q2-1')">
                        <div class="milestone-content">
                            <div class="milestone-title">Launch First Digital Product</div>
                            <div class="milestone-description">3D Design Quote Calculator or AutoCAD Template Library</div>
                            <span class="power-badge power-build">Build</span>
                            <span class="milestone-metric">Product Launch</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q2-2')">
                        <input type="checkbox" class="milestone-checkbox" id="q2-2" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q2-2')">
                        <div class="milestone-content">
                            <div class="milestone-title">Build Portfolio + Booking System</div>
                            <div class="milestone-description">Professional site with AI chatbot for client inquiries</div>
                            <span class="power-badge power-build">Build</span>
                            <span class="milestone-metric">Live Website</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q2-3')">
                        <input type="checkbox" class="milestone-checkbox" id="q2-3" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q2-3')">
                        <div class="milestone-content">
                            <div class="milestone-title">Start YouTube Channel</div>
                            <div class="milestone-description">Launch with 8 tutorials on "AI for Engineers & Designers"</div>
                            <span class="power-badge power-create">Create</span>
                            <span class="milestone-metric">8 Videos</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q2-4')">
                        <input type="checkbox" class="milestone-checkbox" id="q2-4" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q2-4')">
                        <div class="milestone-content">
                            <div class="milestone-title">Create AI-Enhanced Design Templates</div>
                            <div class="milestone-description">Build 20 templates for Gumroad/Etsy using AI tools</div>
                            <span class="power-badge power-create">Create</span>
                            <span class="milestone-metric">20 Templates</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q2-5')">
                        <input type="checkbox" class="milestone-checkbox" id="q2-5" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q2-5')">
                        <div class="milestone-content">
                            <div class="milestone-title">Generate £500 Monthly Passive Income</div>
                            <div class="milestone-description">From digital products, templates, or automation services</div>
                            <span class="power-badge power-build">Build</span>
                            <span class="milestone-metric">£500/month</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q2-6')">
                        <input type="checkbox" class="milestone-checkbox" id="q2-6" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q2-6')">
                        <div class="milestone-content">
                            <div class="milestone-title">Master Video Creation with AI</div>
                            <div class="milestone-description">Use RunwayML, Pika for client presentations and content</div>
                            <span class="power-badge power-create">Create</span>
                            <span class="milestone-metric">Video Skills</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q2-7')">
                        <input type="checkbox" class="milestone-checkbox" id="q2-7" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q2-7')">
                        <div class="milestone-content">
                            <div class="milestone-title">Publish Weekly LinkedIn Articles</div>
                            <div class="milestone-description">Share case studies and AI workflow insights</div>
                            <span class="power-badge power-connect">Connect</span>
                            <span class="milestone-metric">12 Articles</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q2-8')">
                        <input type="checkbox" class="milestone-checkbox" id="q2-8" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q2-8')">
                        <div class="milestone-content">
                            <div class="milestone-title">Land 3 Freelance Clients</div>
                            <div class="milestone-description">Using AI-powered proposals and LinkedIn outreach</div>
                            <span class="power-badge power-connect">Connect</span>
                            <span class="milestone-metric">3 Clients</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q2-9')">
                        <input type="checkbox" class="milestone-checkbox" id="q2-9" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q2-9')">
                        <div class="milestone-content">
                            <div class="milestone-title">Reach 1,500 LinkedIn Followers</div>
                            <div class="milestone-description">Triple your audience through consistent value delivery</div>
                            <span class="power-badge power-connect">Connect</span>
                            <span class="milestone-metric">1,500 followers</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Q3 2025 -->
            <div class="roadmap-quarter">
                <div class="quarter-header">
                    <div class="quarter-title">Q3 2025</div>
                    <div class="quarter-dates">July - September 2025</div>
                </div>
                <div class="quarter-focus">
                    <div class="focus-label">Focus</div>
                    <div class="focus-text">Scale + Connect - Grow income and build authority</div>
                </div>
                <div class="milestone-list">
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q3-1')">
                        <input type="checkbox" class="milestone-checkbox" id="q3-1" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q3-1')">
                        <div class="milestone-content">
                            <div class="milestone-title">Launch Second Major Product</div>
                            <div class="milestone-description">Automation workflow marketplace or advanced template library</div>
                            <span class="power-badge power-build">Build</span>
                            <span class="milestone-metric">Product #2</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q3-2')">
                        <input type="checkbox" class="milestone-checkbox" id="q3-2" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q3-2')">
                        <div class="milestone-content">
                            <div class="milestone-title">Achieve £1,000 Monthly Income</div>
                            <div class="milestone-description">From combined products, services, and content</div>
                            <span class="power-badge power-build">Build</span>
                            <span class="milestone-metric">£1,000/month</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q3-3')">
                        <input type="checkbox" class="milestone-checkbox" id="q3-3" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q3-3')">
                        <div class="milestone-content">
                            <div class="milestone-title">Build Email Newsletter List</div>
                            <div class="milestone-description">500+ subscribers receiving weekly AI insights</div>
                            <span class="power-badge power-connect">Connect</span>
                            <span class="milestone-metric">500 subscribers</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q3-4')">
                        <input type="checkbox" class="milestone-checkbox" id="q3-4" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q3-4')">
                        <div class="milestone-content">
                            <div class="milestone-title">Speak at Local Meetup/Webinar</div>
                            <div class="milestone-description">Present on "AI Workflows for Design Professionals"</div>
                            <span class="power-badge power-connect">Connect</span>
                            <span class="milestone-metric">Speaking Gig</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q3-5')">
                        <input type="checkbox" class="milestone-checkbox" id="q3-5" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q3-5')">
                        <div class="milestone-content">
                            <div class="milestone-title">Create Advanced Prompt Library</div>
                            <div class="milestone-description">50+ proven prompts for engineering and creative work</div>
                            <span class="power-badge power-connect">Connect</span>
                            <span class="milestone-metric">50 Prompts</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q3-6')">
                        <input type="checkbox" class="milestone-checkbox" id="q3-6" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q3-6')">
                        <div class="milestone-content">
                            <div class="milestone-title">Produce 50+ YouTube Videos</div>
                            <div class="milestone-description">Consistent weekly uploads building authority</div>
                            <span class="power-badge power-create">Create</span>
                            <span class="milestone-metric">50 Videos Total</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q3-7')">
                        <input type="checkbox" class="milestone-checkbox" id="q3-7" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q3-7')">
                        <div class="milestone-content">
                            <div class="milestone-title">Automate Content Production</div>
                            <div class="milestone-description">AI-powered system for creating posts, videos, and graphics</div>
                            <span class="power-badge power-automate">Automate</span>
                            <span class="milestone-metric">Content System</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q3-8')">
                        <input type="checkbox" class="milestone-checkbox" id="q3-8" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q3-8')">
                        <div class="milestone-content">
                            <div class="milestone-title">Reach 3,000 LinkedIn Followers</div>
                            <div class="milestone-description">Establish yourself as recognized voice in AI + engineering</div>
                            <span class="power-badge power-connect">Connect</span>
                            <span class="milestone-metric">3,000 followers</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Q4 2025 -->
            <div class="roadmap-quarter">
                <div class="quarter-header">
                    <div class="quarter-title">Q4 2025</div>
                    <div class="quarter-dates">October - December 2025</div>
                </div>
                <div class="quarter-focus">
                    <div class="focus-label">Focus</div>
                    <div class="focus-text">Authority + Stack - Become recognized expert, scale to £3K+/month</div>
                </div>
                <div class="milestone-list">
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q4-1')">
                        <input type="checkbox" class="milestone-checkbox" id="q4-1" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q4-1')">
                        <div class="milestone-content">
                            <div class="milestone-title">Launch Premium Consulting Offer</div>
                            <div class="milestone-description">High-ticket service (£500-£2,000 per project) for AI implementation</div>
                            <span class="power-badge power-connect">Connect</span>
                            <span class="milestone-metric">Consulting Service</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q4-2')">
                        <input type="checkbox" class="milestone-checkbox" id="q4-2" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q4-2')">
                        <div class="milestone-content">
                            <div class="milestone-title">Achieve £3,000+ Monthly Income</div>
                            <div class="milestone-description">Multiple streams: products, consulting, content, services</div>
                            <span class="power-badge power-build">Build</span>
                            <span class="milestone-metric">£3,000/month</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q4-3')">
                        <input type="checkbox" class="milestone-checkbox" id="q4-3" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q4-3')">
                        <div class="milestone-content">
                            <div class="milestone-title">Build Community Platform</div>
                            <div class="milestone-description">Discord or Circle community for engineers learning AI</div>
                            <span class="power-badge power-connect">Connect</span>
                            <span class="milestone-metric">Community</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q4-4')">
                        <input type="checkbox" class="milestone-checkbox" id="q4-4" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q4-4')">
                        <div class="milestone-content">
                            <div class="milestone-title">Launch Course or Coaching Program</div>
                            <div class="milestone-description">"AI for 3D Designers" or similar niche offering</div>
                            <span class="power-badge power-build">Build</span>
                            <span class="milestone-metric">Course Launch</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q4-5')">
                        <input type="checkbox" class="milestone-checkbox" id="q4-5" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q4-5')">
                        <div class="milestone-content">
                            <div class="milestone-title">Guest Post on Industry Blogs</div>
                            <div class="milestone-description">3+ published articles on major design/engineering platforms</div>
                            <span class="power-badge power-connect">Connect</span>
                            <span class="milestone-metric">3 Publications</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q4-6')">
                        <input type="checkbox" class="milestone-checkbox" id="q4-6" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q4-6')">
                        <div class="milestone-content">
                            <div class="milestone-title">Secure Partnership/Sponsorship</div>
                            <div class="milestone-description">Brand partnership for content or product promotion</div>
                            <span class="power-badge power-connect">Connect</span>
                            <span class="milestone-metric">Partnership</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q4-7')">
                        <input type="checkbox" class="milestone-checkbox" id="q4-7" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q4-7')">
                        <div class="milestone-content">
                            <div class="milestone-title">Produce Signature Content Piece</div>
                            <div class="milestone-description">Major case study, documentary, or comprehensive guide</div>
                            <span class="power-badge power-create">Create</span>
                            <span class="milestone-metric">Signature Work</span>
                        </div>
                    </div>
                    <div class="milestone-item" onclick="toggleMilestone(this, 'q4-8')">
                        <input type="checkbox" class="milestone-checkbox" id="q4-8" onclick="event.stopPropagation(); toggleMilestone(this.parentElement, 'q4-8')">
                        <div class="milestone-content">
                            <div class="milestone-title">Reach 5,000+ LinkedIn Followers</div>
                            <div class="milestone-description">Recognized as go-to AI expert in your niche</div>
                            <span class="power-badge power-connect">Connect</span>
                            <span class="milestone-metric">5,000 followers</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- End Roadmap Page -->

        <!-- Achievements Page -->
        <div id="achievementsPage" class="page">
            <!-- Main Content -->
            <div class="main-content">
                <!-- Add Achievement Panel -->
                <div class="panel">
                    <h2>Add New Achievement</h2>
                    <form id="achievementForm">
                        <div class="form-group">
                            <label for="achievementType">Type</label>
                            <select id="achievementType" required>
                                <option value="">Select Type...</option>
                                <option value="linkedin">LinkedIn Post</option>
                                <option value="project">Project Built</option>
                                <option value="course">Course Progress</option>
                                <option value="milestone">Milestone</option>
                            </select>
                        </div>

                        <div class="form-group">
                            <label for="achievementTitle">Title</label>
                            <input type="text" id="achievementTitle" placeholder="e.g., Created Conveyor Automation Tool" required>
                        </div>

                        <div class="form-group">
                            <label for="achievementDescription">Description</label>
                            <textarea id="achievementDescription" placeholder="Add details about your achievement..." required></textarea>
                        </div>

                        <div class="form-group">
                            <label for="achievementLink">Link (Optional)</label>
                            <input type="url" id="achievementLink" placeholder="https://linkedin.com/posts/...">
                        </div>

                        <div class="form-group">
                            <label for="achievementDate">Date</label>
                            <input type="date" id="achievementDate" required>
                        </div>

                        <button type="submit" class="btn">Add Achievement</button>
                    </form>

                    <button class="btn export-btn" onclick="exportData()">Export Data</button>
                    <button class="btn import-btn" onclick="document.getElementById('importFile').click()">Import Data</button>
                    <input type="file" id="importFile" accept=".json" style="display: none;" onchange="importData(event)">
                </div>

                <!-- Achievements List Panel -->
                <div class="panel">
                    <h2>Your Achievements</h2>
                    
                    <!-- Filter Tabs -->
                    <div class="tabs">
                        <button class="tab active" onclick="filterAchievements('all')">All</button>
                        <button class="tab" onclick="filterAchievements('linkedin')">LinkedIn</button>
                        <button class="tab" onclick="filterAchievements('project')">Projects</button>
                        <button class="tab" onclick="filterAchievements('course')">Course</button>
                        <button class="tab" onclick="filterAchievements('milestone')">Milestones</button>
                    </div>

                    <div id="achievementsList"></div>
                </div>
            </div>
        </div>
        <!-- End Achievements Page -->

    </div>

    <script>
        // Page Navigation
        function switchPage(pageName) {
            // Hide all pages
            document.querySelectorAll('.page').forEach(page => page.classList.remove('active'));
            
            // Remove active from all nav tabs
            document.querySelectorAll('.nav-tab').forEach(tab => tab.classList.remove('active'));
            
            // Show selected page
            document.getElementById(pageName + 'Page').classList.add('active');
            
            // Activate corresponding nav tab
            event.target.classList.add('active');
            
            // Update daily date if on roadmap page
            if (pageName === 'roadmap') {
                updateTodayDate();
                loadDailyProgress();
                updateRoadmapProgress();
            }
        }

        // Today's Date
        function updateTodayDate() {
            const options = { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric' };
            document.getElementById('todayDate').textContent = new Date().toLocaleDateString('en-GB', options);
        }

        // Daily Tasks Progress
        function saveDailyProgress() {
            const tasks = {};
            for (let i = 1; i <= 5; i++) {
                tasks[`task${i}`] = document.getElementById(`task${i}`).checked;
            }
            const today = new Date().toISOString().split('T')[0];
            localStorage.setItem(`daily-${today}`, JSON.stringify(tasks));
        }

        function loadDailyProgress() {
            const today = new Date().toISOString().split('T')[0];
            const saved = localStorage.getItem(`daily-${today}`);
            if (saved) {
                const tasks = JSON.parse(saved);
                for (let i = 1; i <= 5; i++) {
                    const checkbox = document.getElementById(`task${i}`);
                    if (checkbox) checkbox.checked = tasks[`task${i}`] || false;
                }
            }
        }

        // Milestone Tracking
        function toggleMilestone(element, id) {
            const checkbox = document.getElementById(id);
            checkbox.checked = !checkbox.checked;
            
            if (checkbox.checked) {
                element.classList.add('completed');
            } else {
                element.classList.remove('completed');
            }
            
            saveMilestones();
            updateRoadmapProgress();
        }

        function saveMilestones() {
            const milestones = {};
            document.querySelectorAll('.milestone-checkbox').forEach(checkbox => {
                milestones[checkbox.id] = checkbox.checked;
            });
            localStorage.setItem('milestones', JSON.stringify(milestones));
        }

        function loadMilestones() {
            const saved = localStorage.getItem('milestones');
            if (saved) {
                const milestones = JSON.parse(saved);
                Object.keys(milestones).forEach(id => {
                    const checkbox = document.getElementById(id);
                    if (checkbox) {
                        checkbox.checked = milestones[id];
                        if (milestones[id]) {
                            checkbox.parentElement.classList.add('completed');
                        }
                    }
                });
            }
        }

        function updateRoadmapProgress() {
            // Q1 Progress
            let q1Total = 8;
            let q1Completed = 0;
            for (let i = 1; i <= q1Total; i++) {
                const checkbox = document.getElementById(`q1-${i}`);
                if (checkbox && checkbox.checked) q1Completed++;
            }
            document.getElementById('q1Progress').textContent = `${q1Completed}/${q1Total}`;

            // Q2 Progress
            let q2Total = 9;
            let q2Completed = 0;
            for (let i = 1; i <= q2Total; i++) {
                const checkbox = document.getElementById(`q2-${i}`);
                if (checkbox && checkbox.checked) q2Completed++;
            }
            document.getElementById('q2Progress').textContent = `${q2Completed}/${q2Total}`;

            // Q3 Progress
            let q3Total = 8;
            let q3Completed = 0;
            for (let i = 1; i <= q3Total; i++) {
                const checkbox = document.getElementById(`q3-${i}`);
                if (checkbox && checkbox.checked) q3Completed++;
            }
            document.getElementById('q3Progress').textContent = `${q3Completed}/${q3Total}`;

            // Q4 Progress
            let q4Total = 8;
            let q4Completed = 0;
            for (let i = 1; i <= q4Total; i++) {
                const checkbox = document.getElementById(`q4-${i}`);
                if (checkbox && checkbox.checked) q4Completed++;
            }
            document.getElementById('q4Progress').textContent = `${q4Completed}/${q4Total}`;

            // Total Progress
            const totalMilestones = q1Total + q2Total + q3Total + q4Total;
            const totalCompleted = q1Completed + q2Completed + q3Completed + q4Completed;
            const totalPercent = Math.round((totalCompleted / totalMilestones) * 100);
            document.getElementById('totalProgress').textContent = `${totalPercent}%`;
        }

        // Initialize with your current achievements
        let achievements = [
            {
                id: 1,
                type: 'linkedin',
                title: 'Started LinkedIn Posting',
                description: 'Began regular posting on LinkedIn to build personal brand and share AI journey',
                link: '',
                date: new Date().toISOString().split('T')[0]
            },
            {
                id: 2,
                type: 'project',
                title: 'Conveyor Automation & Rates Toolkit',
                description: 'Built comprehensive conveyor automation and rates calculation tool using Replit and Lovable',
                link: '',
                date: new Date().toISOString().split('T')[0]
            },
            {
                id: 3,
                type: 'course',
                title: 'AAA Accelerator - Lesson 1.3',
                description: 'Completed up to Lesson 1.3: Field Work in the Foundation section',
                link: '',
                date: new Date().toISOString().split('T')[0]
            }
        ];

        let currentFilter = 'all';

        // Load achievements from localStorage
        function loadAchievements() {
            const stored = localStorage.getItem('achievements');
            if (stored) {
                achievements = JSON.parse(stored);
            }
        }

        // Save achievements to localStorage
        function saveAchievements() {
            localStorage.setItem('achievements', JSON.stringify(achievements));
        }

        // Initialize
        loadAchievements();
        loadMilestones();
        renderAchievements();
        updateStats();
        updateTodayDate();
        loadDailyProgress();

        // Set today's date as default
        document.getElementById('achievementDate').valueAsDate = new Date();

        // Form submission
        document.getElementById('achievementForm').addEventListener('submit', function(e) {
            e.preventDefault();

            const newAchievement = {
                id: Date.now(),
                type: document.getElementById('achievementType').value,
                title: document.getElementById('achievementTitle').value,
                description: document.getElementById('achievementDescription').value,
                link: document.getElementById('achievementLink').value,
                date: document.getElementById('achievementDate').value
            };

            achievements.unshift(newAchievement);
            saveAchievements();
            renderAchievements();
            updateStats();
            this.reset();
            document.getElementById('achievementDate').valueAsDate = new Date();
        });

        function renderAchievements() {
            const container = document.getElementById('achievementsList');
            
            let filtered = achievements;
            if (currentFilter !== 'all') {
                filtered = achievements.filter(a => a.type === currentFilter);
            }

            if (filtered.length === 0) {
                container.innerHTML = '<p style="color: #999; text-align: center; padding: 40px;">No achievements yet. Start adding your wins!</p>';
                return;
            }

            container.innerHTML = filtered.map(achievement => `
                <div class="achievement-item">
                    <div class="achievement-header">
                        <span class="achievement-type type-${achievement.type}">${achievement.type}</span>
                        <span class="achievement-date">${formatDate(achievement.date)}</span>
                    </div>
                    <div class="achievement-title">${achievement.title}</div>
                    <div class="achievement-description">${achievement.description}</div>
                    ${achievement.link ? `<a href="${achievement.link}" target="_blank" class="achievement-link">View Link →</a>` : ''}
                    <div style="margin-top: 10px;">
                        <button class="delete-btn" onclick="deleteAchievement(${achievement.id})">Delete</button>
                    </div>
                </div>
            `).join('');
        }

        function deleteAchievement(id) {
            if (confirm('Are you sure you want to delete this achievement?')) {
                achievements = achievements.filter(a => a.id !== id);
                saveAchievements();
                renderAchievements();
                updateStats();
            }
        }

        function updateStats() {
            const linkedinCount = achievements.filter(a => a.type === 'linkedin').length;
            const projectCount = achievements.filter(a => a.type === 'project').length;

            document.getElementById('totalAchievements').textContent = achievements.length;
            document.getElementById('linkedinPosts').textContent = linkedinCount;
            document.getElementById('projectsBuilt').textContent = projectCount;
        }

        function formatDate(dateString) {
            const options = { year: 'numeric', month: 'short', day: 'numeric' };
            return new Date(dateString).toLocaleDateString('en-GB', options);
        }

        function filterAchievements(type) {
            currentFilter = type;
            
            // Update tab active state
            document.querySelectorAll('.tab').forEach(tab => tab.classList.remove('active'));
            event.target.classList.add('active');
            
            renderAchievements();
        }

        function updateCourseProgress() {
            const progress = prompt('Enter your current course completion percentage (0-100):', '5');
            if (progress !== null) {
                const progressNum = Math.min(100, Math.max(0, parseInt(progress) || 0));
                document.getElementById('courseProgress').textContent = progressNum + '%';
                document.getElementById('courseProgressBar').style.width = progressNum + '%';
                document.getElementById('courseProgressBar').textContent = progressNum + '%';
                localStorage.setItem('courseProgress', progressNum);
            }
        }

        // Load course progress
        const savedProgress = localStorage.getItem('courseProgress');
        if (savedProgress) {
            document.getElementById('courseProgress').textContent = savedProgress + '%';
            document.getElementById('courseProgressBar').style.width = savedProgress + '%';
            document.getElementById('courseProgressBar').textContent = savedProgress + '%';
        }

        function exportData() {
            const data = {
                achievements: achievements,
                courseProgress: localStorage.getItem('courseProgress') || '5',
                milestones: JSON.parse(localStorage.getItem('milestones') || '{}'),
                exportDate: new Date().toISOString()
            };

            const blob = new Blob([JSON.stringify(data, null, 2)], { type: 'application/json' });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = `errol-ai-progress-${new Date().toISOString().split('T')[0]}.json`;
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            URL.revokeObjectURL(url);
        }

        function importData(event) {
            const file = event.target.files[0];
            if (file) {
                const reader = new FileReader();
                reader.onload = function(e) {
                    try {
                        const data = JSON.parse(e.target.result);
                        if (confirm('This will replace your current data. Continue?')) {
                            achievements = data.achievements || [];
                            if (data.courseProgress) {
                                localStorage.setItem('courseProgress', data.courseProgress);
                                document.getElementById('courseProgress').textContent = data.courseProgress + '%';
                                document.getElementById('courseProgressBar').style.width = data.courseProgress + '%';
                                document.getElementById('courseProgressBar').textContent = data.courseProgress + '%';
                            }
                            if (data.milestones) {
                                localStorage.setItem('milestones', JSON.stringify(data.milestones));
                                loadMilestones();
                                updateRoadmapProgress();
                            }
                            saveAchievements();
                            renderAchievements();
                            updateStats();
                            alert('Data imported successfully!');
                        }
                    } catch (error) {
                        alert('Error importing data. Please check the file format.');
                    }
                };
                reader.readAsText(file);
            }
        }
    </script>
</body>
</html>
