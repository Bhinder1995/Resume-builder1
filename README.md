# Resume-builder1
A Web application for creating professional resumes
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Resume Creator | Build Your Perfect Resume</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Inter:wght@300;400;500&display=swap" rel="stylesheet">
    <link rel="icon" type="image/x-icon" href="assets/favicon.ico">
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar">
        <div class="nav-container">
            <div class="logo">
                <i class="fas fa-file-alt"></i>
                <h1>Resume Creator</h1>
            </div>
            <div class="nav-links">
                <a href="#" class="active"><i class="fas fa-home"></i> Home</a>
                <a href="#templates"><i class="fas fa-palette"></i> Templates</a>
                <a href="#builder"><i class="fas fa-edit"></i> Builder</a>
                <a href="#preview"><i class="fas fa-eye"></i> Preview</a>
                <div class="user-actions">
                    <button class="btn-login"><i class="fas fa-user"></i> Login</button>
                    <div class="credits-display">
                        <i class="fas fa-coins"></i>
                        <span id="credits">3</span> Free Credits
                    </div>
                </div>
            </div>
            <button class="menu-toggle">
                <i class="fas fa-bars"></i>
            </button>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-container">
            <div class="hero-content">
                <h2>Create a Professional Resume in <span class="highlight">5 Minutes</span></h2>
                <p class="subtitle">ATS-friendly templates designed for Indian job market. Free to start, unlock more with ads.</p>
                <div class="hero-stats">
                    <div class="stat">
                        <i class="fas fa-users"></i>
                        <div>
                            <h3>10,000+</h3>
                            <p>Resumes Created</p>
                        </div>
                    </div>
                    <div class="stat">
                        <i class="fas fa-thumbs-up"></i>
                        <div>
                            <h3>95%</h3>
                            <p>ATS Success Rate</p>
                        </div>
                    </div>
                    <div class="stat">
                        <i class="fas fa-bolt"></i>
                        <div>
                            <h3>5 Min</h3>
                            <p>Average Time</p>
                        </div>
                    </div>
                </div>
                <a href="#builder" class="btn-primary">
                    <i class="fas fa-rocket"></i> Start Building Free
                </a>
            </div>
            <div class="hero-image">
                <div class="resume-preview">
                    <div class="preview-header"></div>
                    <div class="preview-content">
                        <div class="preview-line"></div>
                        <div class="preview-line short"></div>
                        <div class="preview-line"></div>
                        <div class="preview-line short"></div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Templates Section -->
    <section id="templates" class="templates-section">
        <div class="container">
            <div class="section-header">
                <h2>Choose Your Perfect Template</h2>
                <p>Start with free templates or unlock premium with ads</p>
                <div class="credits-info">
                    <i class="fas fa-info-circle"></i>
                    <span>You have <strong id="credits-count">3</strong> free template credits. Watch ads to unlock more.</span>
                </div>
            </div>

            <div class="template-filters">
                <button class="filter-btn active" data-filter="all">All Templates</button>
                <button class="filter-btn" data-filter="free">Free</button>
                <button class="filter-btn" data-filter="premium">Premium</button>
                <button class="filter-btn" data-filter="fresher">Fresher</button>
                <button class="filter-btn" data-filter="experienced">Experienced</button>
            </div>

            <div class="templates-grid">
                <!-- Template 1 - Free -->
                <div class="template-card" data-category="free fresher">
                    <div class="template-badge free">FREE</div>
                    <div class="template-preview" style="background: linear-gradient(135deg, #4f6df5 0%, #3a56d5 100%);">
                        <div class="template-placeholder">
                            <div class="tp-header"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line short"></div>
                            <div class="tp-line"></div>
                        </div>
                    </div>
                    <div class="template-info">
                        <h3>Modern Blue</h3>
                        <p>Clean & professional for freshers</p>
                        <div class="template-tags">
                            <span class="tag">ATS Friendly</span>
                            <span class="tag">Single Page</span>
                        </div>
                        <button class="btn-use-template" data-template="1">
                            <i class="fas fa-magic"></i> Use Template
                        </button>
                    </div>
                </div>

                <!-- Template 2 - Free -->
                <div class="template-card" data-category="free experienced">
                    <div class="template-badge free">FREE</div>
                    <div class="template-preview" style="background: linear-gradient(135deg, #10b981 0%, #059669 100%);">
                        <div class="template-placeholder">
                            <div class="tp-header"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line short"></div>
                        </div>
                    </div>
                    <div class="template-info">
                        <h3>Professional Green</h3>
                        <p>Experienced professionals</p>
                        <div class="template-tags">
                            <span class="tag">Corporate</span>
                            <span class="tag">Detailed</span>
                        </div>
                        <button class="btn-use-template" data-template="2">
                            <i class="fas fa-magic"></i> Use Template
                        </button>
                    </div>
                </div>

                <!-- Template 3 - Free -->
                <div class="template-card" data-category="free fresher">
                    <div class="template-badge free">FREE</div>
                    <div class="template-preview" style="background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%);">
                        <div class="template-placeholder">
                            <div class="tp-header"></div>
                            <div class="tp-line short"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line short"></div>
                        </div>
                    </div>
                    <div class="template-info">
                        <h3>Creative Purple</h3>
                        <p>Design & creative fields</p>
                        <div class="template-tags">
                            <span class="tag">Creative</span>
                            <span class="tag">Modern</span>
                        </div>
                        <button class="btn-use-template" data-template="3">
                            <i class="fas fa-magic"></i> Use Template
                        </button>
                    </div>
                </div>

                <!-- Template 4 - Premium (Ad Required) -->
                <div class="template-card" data-category="premium experienced">
                    <div class="template-badge premium">PREMIUM</div>
                    <div class="template-preview" style="background: linear-gradient(135deg, #f59e0b 0%, #d97706 100%);">
                        <div class="template-placeholder">
                            <div class="tp-header gold"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line short"></div>
                            <div class="tp-line"></div>
                        </div>
                    </div>
                    <div class="template-info">
                        <h3>Executive Gold</h3>
                        <p>Senior level & executives</p>
                        <div class="template-tags">
                            <span class="tag">Executive</span>
                            <span class="tag">Premium</span>
                        </div>
                        <button class="btn-use-template premium-locked" data-template="4">
                            <i class="fas fa-lock"></i> Watch Ad to Unlock
                        </button>
                    </div>
                </div>

                <!-- Template 5 - Premium (Ad Required) -->
                <div class="template-card" data-category="premium fresher">
                    <div class="template-badge premium">PREMIUM</div>
                    <div class="template-preview" style="background: linear-gradient(135deg, #ec4899 0%, #db2777 100%);">
                        <div class="template-placeholder">
                            <div class="tp-header"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line short"></div>
                        </div>
                    </div>
                    <div class="template-info">
                        <h3>Minimal Pink</h3>
                        <p>Minimalist & elegant</p>
                        <div class="template-tags">
                            <span class="tag">Minimal</span>
                            <span class="tag">Elegant</span>
                        </div>
                        <button class="btn-use-template premium-locked" data-template="5">
                            <i class="fas fa-lock"></i> Watch Ad to Unlock
                        </button>
                    </div>
                </div>

                <!-- Template 6 - Premium (Ad Required) -->
                <div class="template-card" data-category="premium experienced">
                    <div class="template-badge premium">PREMIUM</div>
                    <div class="template-preview" style="background: linear-gradient(135deg, #0ea5e9 0%, #0284c7 100%);">
                        <div class="template-placeholder">
                            <div class="tp-header"></div>
                            <div class="tp-line short"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line short"></div>
                        </div>
                    </div>
                    <div class="template-info">
                        <h3>Corporate Blue</h3>
                        <p>Traditional corporate style</p>
                        <div class="template-tags">
                            <span class="tag">Traditional</span>
                            <span class="tag">Formal</span>
                        </div>
                        <button class="btn-use-template premium-locked" data-template="6">
                            <i class="fas fa-lock"></i> Watch Ad to Unlock
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Resume Builder Section -->
    <section id="builder" class="builder-section">
        <div class="container">
            <div class="section-header">
                <h2>Build Your Resume</h2>
                <p>Fill in your details and watch your resume come to life</p>
            </div>

            <div class="builder-container">
                <!-- Form Section -->
                <div class="form-section">
                    <div class="form-tabs">
                        <button class="form-tab active" data-tab="personal">
                            <i class="fas fa-user"></i> Personal
                        </button>
                        <button class="form-tab" data-tab="education">
                            <i class="fas fa-graduation-cap"></i> Education
                        </button>
                        <button class="form-tab" data-tab="experience">
                            <i class="fas fa-briefcase"></i> Experience
                        </button>
                        <button class="form-tab" data-tab="skills">
                            <i class="fas fa-star"></i> Skills
                        </button>
                        <button class="form-tab" data-tab="customize">
                            <i class="fas fa-palette"></i> Customize
                        </button>
                    </div>

                    <div class="form-content">
                        <!-- Personal Info Tab -->
                        <div class="tab-pane active" id="personal-tab">
                            <h3><i class="fas fa-user-circle"></i> Personal Information</h3>
                            <div class="form-group">
                                <label for="fullName"><i class="fas fa-signature"></i> Full Name</label>
                                <input type="text" id="fullName" placeholder="Enter your full name">
                            </div>
                            <div class="form-row">
                                <div class="form-group">
                                    <label for="jobTitle"><i class="fas fa-briefcase"></i> Job Title</label>
                                    <input type="text" id="jobTitle" placeholder="e.g., Software Developer">
                                </div>
                                <div class="form-group">
                                    <label for="phone"><i class="fas fa-phone"></i> Phone</label>
                                    <input type="tel" id="phone" placeholder="+91 98765 43210">
                                </div>
                            </div>
                            <div class="form-group">
                                <label for="email"><i class="fas fa-envelope"></i> Email</label>
                                <input type="email" id="email" placeholder="your.email@example.com">
                            </div>
                            <div class="form-group">
                                <label for="location"><i class="fas fa-map-marker-alt"></i> Location</label>
                                <input type="text" id="location" placeholder="City, State">
                            </div>
                            <div class="form-group">
                                <label for="linkedin"><i class="fab fa-linkedin"></i> LinkedIn Profile (Optional)</label>
                                <input type="url" id="linkedin" placeholder="https://linkedin.com/in/yourprofile">
                            </div>
                            <div class="form-group">
                                <label for="summary"><i class="fas fa-file-alt"></i> Professional Summary</label>
                                <textarea id="summary" rows="4" placeholder="Brief summary of your professional background and career objectives..."></textarea>
                                <div class="char-count">0/200 characters</div>
                            </div>
                        </div>

                        <!-- Education Tab -->
                        <div class="tab-pane" id="education-tab">
                            <h3><i class="fas fa-graduation-cap"></i> Education</h3>
                            <div class="dynamic-section" id="education-section">
                                <!-- Education entries will be added here -->
                            </div>
                            <button class="btn-add-section" id="add-education">
                                <i class="fas fa-plus"></i> Add Education
                            </button>
                        </div>

                        <!-- Experience Tab -->
                        <div class="tab-pane" id="experience-tab">
                            <h3><i class="fas fa-briefcase"></i> Work Experience</h3>
                            <div class="dynamic-section" id="experience-section">
                                <!-- Experience entries will be added here -->
                            </div>
                            <button class="btn-add-section" id="add-experience">
                                <i class="fas fa-plus"></i> Add Experience
                            </button>
                        </div>

                        <!-- Skills Tab -->
                        <div class="tab-pane" id="skills-tab">
                            <h3><i class="fas fa-star"></i> Skills</h3>
                            <div class="skills-container">
                                <div class="skills-input">
                                    <input type="text" id="skill-input" placeholder="Type a skill and press Enter">
                                    <button id="add-skill"><i class="fas fa-plus"></i> Add</button>
                                </div>
                                <div class="skills-tags" id="skills-list">
                                    <!-- Skills will appear here as tags -->
                                    <span class="skill-tag">JavaScript <i class="fas fa-times remove-skill"></i></span>
                                    <span class="skill-tag">React <i class="fas fa-times remove-skill"></i></span>
                                    <span class="skill-tag">Python <i class="fas fa-times remove-skill"></i></span>
                                </div>
                                <div class="skill-suggestions">
                                    <p>Suggestions: </p>
                                    <span class="skill-suggestion">HTML/CSS</span>
                                    <span class="skill-suggestion">Node.js</span>
                                    <span class="skill-suggestion">SQL</span>
                                    <span class="skill-suggestion">Communication</span>
                                    <span class="skill-suggestion">Team Leadership</span>
                                </div>
                            </div>
                        </div>

                        <!-- Customize Tab -->
                        <div class="tab-pane" id="customize-tab">
                            <h3><i class="fas fa-palette"></i> Customize Design</h3>
                            <div class="form-group">
                                <label><i class="fas fa-font"></i> Font Family</label>
                                <select id="fontFamily" class="form-select">
                                    <option value="Inter, sans-serif">Inter (Modern)</option>
                                    <option value="Poppins, sans-serif">Poppins (Professional)</option>
                                    <option value="Georgia, serif">Georgia (Traditional)</option>
                                    <option value="Arial, sans-serif">Arial (Clean)</option>
                                </select>
                            </div>
                            <div class="form-group">
                                <label><i class="fas fa-paint-brush"></i> Color Scheme</label>
                                <div class="color-options">
                                    <div class="color-option" data-color="#4f6df5" style="background-color: #4f6df5;"></div>
                                    <div class="color-option" data-color="#10b981" style="background-color: #10b981;"></div>
                                    <div class="color-option" data-color="#8b5cf6" style="background-color: #8b5cf6;"></div>
                                    <div class="color-option" data-color="#f59e0b" style="background-color: #f59e0b;"></div>
                                    <div class="color-option" data-color="#ec4899" style="background-color: #ec4899;"></div>
                                    <div class="color-option" data-color="#0ea5e9" style="background-color: #0ea5e9;"></div>
                                </div>
                            </div>
                            <div class="form-group">
                                <label><i class="fas fa-columns"></i> Layout</label>
                                <div class="layout-options">
                                    <div class="layout-option active" data-layout="single">
                                        <i class="fas fa-file-alt"></i>
                                        <span>Single Column</span>
                                    </div>
                                    <div class="layout-option" data-layout="double">
                                        <i class="fas fa-columns"></i>
                                        <span>Two Column</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="form-actions">
                        <button class="btn-secondary" id="reset-form">
                            <i class="fas fa-redo"></i> Reset All
                        </button>
                        <button class="btn-primary" id="generate-resume">
                            <i class="fas fa-file-pdf"></i> Generate & Download PDF
                        </button>
                    </div>
                </div>

                <!-- Live Preview Section -->
                <div class="preview-section">
                    <div class="preview-header">
                        <h3><i class="fas fa-eye"></i> Live Preview</h3>
                        <div class="preview-actions">
                            <button class="btn-icon" id="zoom-in"><i class="fas fa-search-plus"></i></button>
                            <button class="btn-icon" id="zoom-out"><i class="fas fa-search-minus"></i></button>
                            <button class="btn-icon" id="toggle-preview"><i class="fas fa-expand"></i></button>
                        </div>
                    </div>
                    <div class="preview-container">
                        <div class="resume-preview" id="resume-preview">
                            <!-- Resume preview will be rendered here -->
                        </div>
                    </div>
                    <div class="preview-stats">
                        <div class="stat">
                            <i class="fas fa-file-word"></i>
                            <span id="word-count">0</span> words
                        </div>
                        <div class="stat">
                            <i class="fas fa-bullseye"></i>
                            <span id="ats-score">85</span> ATS Score
                        </div>
                        <div class="stat">
                            <i class="fas fa-clock"></i>
                            <span>Auto-saved</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Ad Modal -->
    <div class="modal" id="ad-modal">
        <div class="modal-content">
            <div class="modal-header">
                <h3>Unlock Premium Template</h3>
                <button class="modal-close">&times;</button>
            </div>
            <div class="modal-body">
                <div class="ad-container">
                    <div class="ad-content">
                        <i class="fas fa-ad"></i>
                        <h4>Watch a Short Ad to Continue</h4>
                        <p>Support us by watching a 30-second ad to unlock premium templates.</p>
                        <div class="ad-countdown">
                            <div class="countdown-circle">
                                <span id="countdown">30</span>s
                            </div>
                            <p>Ad will play automatically</p>
                        </div>
                        <div class="ad-placeholder">
                            <div class="ad-video-placeholder">
                                <div class="play-button">
                                    <i class="fas fa-play"></i>
                                </div>
                                <p>Advertisement Video</p>
                            </div>
                        </div>
                        <div class="ad-benefits">
                            <p><i class="fas fa-check-circle"></i> Unlock premium template</p>
                            <p><i class="fas fa-check-circle"></i> Support free service</p>
                            <p><i class="fas fa-check-circle"></i> No payment required</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="modal-footer">
                <button class="btn-secondary" id="skip-ad">Skip Ad (Use Credit)</button>
                <button class="btn-primary" id="watch-ad">Watch Ad to Unlock</button>
            </div>
        </div>
    </div>

    <!-- Success Modal -->
    <div class="modal" id="success-modal">
        <div class="modal-content success-modal">
            <div class="success-icon">
                <i class="fas fa-check-circle"></i>
            </div>
            <h3>Resume Created Successfully!</h3>
            <p>Your professional resume is ready to download.</p>
            <div class="success-actions">
                <button class="btn-secondary" id="edit-again">
                    <i class="fas fa-edit"></i> Edit Again
                </button>
                <button class="btn-primary" id="download-pdf">
                    <i class="fas fa-download"></i> Download PDF
                </button>
                <button class="btn-success" id="share-resume">
                    <i class="fas fa-share-alt"></i> Share
                </button>
            </div>
            <div class="success-tips">
                <h4><i class="fas fa-lightbulb"></i> Pro Tips:</h4>
                <ul>
                    <li>Save your resume with filename: <strong>YourName_Resume.pdf</strong></li>
                    <li>Customize for each job application</li>
                    <li>Keep it to 1-2 pages maximum</li>
                </ul>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <div class="logo">
                        <i class="fas fa-file-alt"></i>
                        <h2>Resume Creator</h2>
                    </div>
                    <p>Creating professional resumes for the Indian job market since 2024.</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-linkedin"></i></a>
                        <a href="#"><i class="fab fa-github"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                    </div>
                </div>
                <div class="footer-section">
                    <h3>Quick Links</h3>
                    <a href="#templates">Templates</a>
                    <a href="#builder">Resume Builder</a>
                    <a href="#">Examples</a>
                    <a href="#">Tips & Guides</a>
                </div>
                <div class="footer-section">
                    <h3>Resources</h3>
                    <a href="#">ATS Guidelines</a>
                    <a href="#">Cover Letter Builder</a>
                    <a href="#">Interview Prep</a>
                    <a href="#">Career Blog</a>
                </div>
                <div class="footer-section">
                    <h3>Legal</h3>
                    <a href="#">Privacy Policy</a>
                    <a href="#">Terms of Service</a>
                    <a href="#">Cookie Policy</a>
                    <a href="#">Contact Us</a>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; 2024 Resume Creator. All rights reserved. | Made with <i class="fas fa-heart"></i> for Indian job seekers</p>
                <p>Free to use • Premium templates via ads • No hidden charges</p>
            </div>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Resume Creator | Build Your Perfect Resume</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Inter:wght@300;400;500&display=swap" rel="stylesheet">
    <link rel="icon" type="image/x-icon" href="assets/favicon.ico">
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar">
        <div class="nav-container">
            <div class="logo">
                <i class="fas fa-file-alt"></i>
                <h1>Resume Creator</h1>
            </div>
            <div class="nav-links">
                <a href="#" class="active"><i class="fas fa-home"></i> Home</a>
                <a href="#templates"><i class="fas fa-palette"></i> Templates</a>
                <a href="#builder"><i class="fas fa-edit"></i> Builder</a>
                <a href="#preview"><i class="fas fa-eye"></i> Preview</a>
                <div class="user-actions">
                    <button class="btn-login"><i class="fas fa-user"></i> Login</button>
                    <div class="credits-display">
                        <i class="fas fa-coins"></i>
                        <span id="credits">3</span> Free Credits
                    </div>
                </div>
            </div>
            <button class="menu-toggle">
                <i class="fas fa-bars"></i>
            </button>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-container">
            <div class="hero-content">
                <h2>Create a Professional Resume in <span class="highlight">5 Minutes</span></h2>
                <p class="subtitle">ATS-friendly templates designed for Indian job market. Free to start, unlock more with ads.</p>
                <div class="hero-stats">
                    <div class="stat">
                        <i class="fas fa-users"></i>
                        <div>
                            <h3>10,000+</h3>
                            <p>Resumes Created</p>
                        </div>
                    </div>
                    <div class="stat">
                        <i class="fas fa-thumbs-up"></i>
                        <div>
                            <h3>95%</h3>
                            <p>ATS Success Rate</p>
                        </div>
                    </div>
                    <div class="stat">
                        <i class="fas fa-bolt"></i>
                        <div>
                            <h3>5 Min</h3>
                            <p>Average Time</p>
                        </div>
                    </div>
                </div>
                <a href="#builder" class="btn-primary">
                    <i class="fas fa-rocket"></i> Start Building Free
                </a>
            </div>
            <div class="hero-image">
                <div class="resume-preview">
                    <div class="preview-header"></div>
                    <div class="preview-content">
                        <div class="preview-line"></div>
                        <div class="preview-line short"></div>
                        <div class="preview-line"></div>
                        <div class="preview-line short"></div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Templates Section -->
    <section id="templates" class="templates-section">
        <div class="container">
            <div class="section-header">
                <h2>Choose Your Perfect Template</h2>
                <p>Start with free templates or unlock premium with ads</p>
                <div class="credits-info">
                    <i class="fas fa-info-circle"></i>
                    <span>You have <strong id="credits-count">3</strong> free template credits. Watch ads to unlock more.</span>
                </div>
            </div>

            <div class="template-filters">
                <button class="filter-btn active" data-filter="all">All Templates</button>
                <button class="filter-btn" data-filter="free">Free</button>
                <button class="filter-btn" data-filter="premium">Premium</button>
                <button class="filter-btn" data-filter="fresher">Fresher</button>
                <button class="filter-btn" data-filter="experienced">Experienced</button>
            </div>

            <div class="templates-grid">
                <!-- Template 1 - Free -->
                <div class="template-card" data-category="free fresher">
                    <div class="template-badge free">FREE</div>
                    <div class="template-preview" style="background: linear-gradient(135deg, #4f6df5 0%, #3a56d5 100%);">
                        <div class="template-placeholder">
                            <div class="tp-header"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line short"></div>
                            <div class="tp-line"></div>
                        </div>
                    </div>
                    <div class="template-info">
                        <h3>Modern Blue</h3>
                        <p>Clean & professional for freshers</p>
                        <div class="template-tags">
                            <span class="tag">ATS Friendly</span>
                            <span class="tag">Single Page</span>
                        </div>
                        <button class="btn-use-template" data-template="1">
                            <i class="fas fa-magic"></i> Use Template
                        </button>
                    </div>
                </div>

                <!-- Template 2 - Free -->
                <div class="template-card" data-category="free experienced">
                    <div class="template-badge free">FREE</div>
                    <div class="template-preview" style="background: linear-gradient(135deg, #10b981 0%, #059669 100%);">
                        <div class="template-placeholder">
                            <div class="tp-header"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line short"></div>
                        </div>
                    </div>
                    <div class="template-info">
                        <h3>Professional Green</h3>
                        <p>Experienced professionals</p>
                        <div class="template-tags">
                            <span class="tag">Corporate</span>
                            <span class="tag">Detailed</span>
                        </div>
                        <button class="btn-use-template" data-template="2">
                            <i class="fas fa-magic"></i> Use Template
                        </button>
                    </div>
                </div>

                <!-- Template 3 - Free -->
                <div class="template-card" data-category="free fresher">
                    <div class="template-badge free">FREE</div>
                    <div class="template-preview" style="background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%);">
                        <div class="template-placeholder">
                            <div class="tp-header"></div>
                            <div class="tp-line short"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line short"></div>
                        </div>
                    </div>
                    <div class="template-info">
                        <h3>Creative Purple</h3>
                        <p>Design & creative fields</p>
                        <div class="template-tags">
                            <span class="tag">Creative</span>
                            <span class="tag">Modern</span>
                        </div>
                        <button class="btn-use-template" data-template="3">
                            <i class="fas fa-magic"></i> Use Template
                        </button>
                    </div>
                </div>

                <!-- Template 4 - Premium (Ad Required) -->
                <div class="template-card" data-category="premium experienced">
                    <div class="template-badge premium">PREMIUM</div>
                    <div class="template-preview" style="background: linear-gradient(135deg, #f59e0b 0%, #d97706 100%);">
                        <div class="template-placeholder">
                            <div class="tp-header gold"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line short"></div>
                            <div class="tp-line"></div>
                        </div>
                    </div>
                    <div class="template-info">
                        <h3>Executive Gold</h3>
                        <p>Senior level & executives</p>
                        <div class="template-tags">
                            <span class="tag">Executive</span>
                            <span class="tag">Premium</span>
                        </div>
                        <button class="btn-use-template premium-locked" data-template="4">
                            <i class="fas fa-lock"></i> Watch Ad to Unlock
                        </button>
                    </div>
                </div>

                <!-- Template 5 - Premium (Ad Required) -->
                <div class="template-card" data-category="premium fresher">
                    <div class="template-badge premium">PREMIUM</div>
                    <div class="template-preview" style="background: linear-gradient(135deg, #ec4899 0%, #db2777 100%);">
                        <div class="template-placeholder">
                            <div class="tp-header"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line short"></div>
                        </div>
                    </div>
                    <div class="template-info">
                        <h3>Minimal Pink</h3>
                        <p>Minimalist & elegant</p>
                        <div class="template-tags">
                            <span class="tag">Minimal</span>
                            <span class="tag">Elegant</span>
                        </div>
                        <button class="btn-use-template premium-locked" data-template="5">
                            <i class="fas fa-lock"></i> Watch Ad to Unlock
                        </button>
                    </div>
                </div>

                <!-- Template 6 - Premium (Ad Required) -->
                <div class="template-card" data-category="premium experienced">
                    <div class="template-badge premium">PREMIUM</div>
                    <div class="template-preview" style="background: linear-gradient(135deg, #0ea5e9 0%, #0284c7 100%);">
                        <div class="template-placeholder">
                            <div class="tp-header"></div>
                            <div class="tp-line short"></div>
                            <div class="tp-line"></div>
                            <div class="tp-line short"></div>
                        </div>
                    </div>
                    <div class="template-info">
                        <h3>Corporate Blue</h3>
                        <p>Traditional corporate style</p>
                        <div class="template-tags">
                            <span class="tag">Traditional</span>
                            <span class="tag">Formal</span>
                        </div>
                        <button class="btn-use-template premium-locked" data-template="6">
                            <i class="fas fa-lock"></i> Watch Ad to Unlock
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Resume Builder Section -->
    <section id="builder" class="builder-section">
        <div class="container">
            <div class="section-header">
                <h2>Build Your Resume</h2>
                <p>Fill in your details and watch your resume come to life</p>
            </div>

            <div class="builder-container">
                <!-- Form Section -->
                <div class="form-section">
                    <div class="form-tabs">
                        <button class="form-tab active" data-tab="personal">
                            <i class="fas fa-user"></i> Personal
                        </button>
                        <button class="form-tab" data-tab="education">
                            <i class="fas fa-graduation-cap"></i> Education
                        </button>
                        <button class="form-tab" data-tab="experience">
                            <i class="fas fa-briefcase"></i> Experience
                        </button>
                        <button class="form-tab" data-tab="skills">
                            <i class="fas fa-star"></i> Skills
                        </button>
                        <button class="form-tab" data-tab="customize">
                            <i class="fas fa-palette"></i> Customize
                        </button>
                    </div>

                    <div class="form-content">
                        <!-- Personal Info Tab -->
                        <div class="tab-pane active" id="personal-tab">
                            <h3><i class="fas fa-user-circle"></i> Personal Information</h3>
                            <div class="form-group">
                                <label for="fullName"><i class="fas fa-signature"></i> Full Name</label>
                                <input type="text" id="fullName" placeholder="Enter your full name">
                            </div>
                            <div class="form-row">
                                <div class="form-group">
                                    <label for="jobTitle"><i class="fas fa-briefcase"></i> Job Title</label>
                                    <input type="text" id="jobTitle" placeholder="e.g., Software Developer">
                                </div>
                                <div class="form-group">
                                    <label for="phone"><i class="fas fa-phone"></i> Phone</label>
                                    <input type="tel" id="phone" placeholder="+91 98765 43210">
                                </div>
                            </div>
                            <div class="form-group">
                                <label for="email"><i class="fas fa-envelope"></i> Email</label>
                                <input type="email" id="email" placeholder="your.email@example.com">
                            </div>
                            <div class="form-group">
                                <label for="location"><i class="fas fa-map-marker-alt"></i> Location</label>
                                <input type="text" id="location" placeholder="City, State">
                            </div>
                            <div class="form-group">
                                <label for="linkedin"><i class="fab fa-linkedin"></i> LinkedIn Profile (Optional)</label>
                                <input type="url" id="linkedin" placeholder="https://linkedin.com/in/yourprofile">
                            </div>
                            <div class="form-group">
                                <label for="summary"><i class="fas fa-file-alt"></i> Professional Summary</label>
                                <textarea id="summary" rows="4" placeholder="Brief summary of your professional background and career objectives..."></textarea>
                                <div class="char-count">0/200 characters</div>
                            </div>
                        </div>

                        <!-- Education Tab -->
                        <div class="tab-pane" id="education-tab">
                            <h3><i class="fas fa-graduation-cap"></i> Education</h3>
                            <div class="dynamic-section" id="education-section">
                                <!-- Education entries will be added here -->
                            </div>
                            <button class="btn-add-section" id="add-education">
                                <i class="fas fa-plus"></i> Add Education
                            </button>
                        </div>

                        <!-- Experience Tab -->
                        <div class="tab-pane" id="experience-tab">
                            <h3><i class="fas fa-briefcase"></i> Work Experience</h3>
                            <div class="dynamic-section" id="experience-section">
                                <!-- Experience entries will be added here -->
                            </div>
                            <button class="btn-add-section" id="add-experience">
                                <i class="fas fa-plus"></i> Add Experience
                            </button>
                        </div>

                        <!-- Skills Tab -->
                        <div class="tab-pane" id="skills-tab">
                            <h3><i class="fas fa-star"></i> Skills</h3>
                            <div class="skills-container">
                                <div class="skills-input">
                                    <input type="text" id="skill-input" placeholder="Type a skill and press Enter">
                                    <button id="add-skill"><i class="fas fa-plus"></i> Add</button>
                                </div>
                                <div class="skills-tags" id="skills-list">
                                    <!-- Skills will appear here as tags -->
                                    <span class="skill-tag">JavaScript <i class="fas fa-times remove-skill"></i></span>
                                    <span class="skill-tag">React <i class="fas fa-times remove-skill"></i></span>
                                    <span class="skill-tag">Python <i class="fas fa-times remove-skill"></i></span>
                                </div>
                                <div class="skill-suggestions">
                                    <p>Suggestions: </p>
                                    <span class="skill-suggestion">HTML/CSS</span>
                                    <span class="skill-suggestion">Node.js</span>
                                    <span class="skill-suggestion">SQL</span>
                                    <span class="skill-suggestion">Communication</span>
                                    <span class="skill-suggestion">Team Leadership</span>
                                </div>
                            </div>
                        </div>

                        <!-- Customize Tab -->
                        <div class="tab-pane" id="customize-tab">
                            <h3><i class="fas fa-palette"></i> Customize Design</h3>
                            <div class="form-group">
                                <label><i class="fas fa-font"></i> Font Family</label>
                                <select id="fontFamily" class="form-select">
                                    <option value="Inter, sans-serif">Inter (Modern)</option>
                                    <option value="Poppins, sans-serif">Poppins (Professional)</option>
                                    <option value="Georgia, serif">Georgia (Traditional)</option>
                                    <option value="Arial, sans-serif">Arial (Clean)</option>
                                </select>
                            </div>
                            <div class="form-group">
                                <label><i class="fas fa-paint-brush"></i> Color Scheme</label>
                                <div class="color-options">
                                    <div class="color-option" data-color="#4f6df5" style="background-color: #4f6df5;"></div>
                                    <div class="color-option" data-color="#10b981" style="background-color: #10b981;"></div>
                                    <div class="color-option" data-color="#8b5cf6" style="background-color: #8b5cf6;"></div>
                                    <div class="color-option" data-color="#f59e0b" style="background-color: #f59e0b;"></div>
                                    <div class="color-option" data-color="#ec4899" style="background-color: #ec4899;"></div>
                                    <div class="color-option" data-color="#0ea5e9" style="background-color: #0ea5e9;"></div>
                                </div>
                            </div>
                            <div class="form-group">
                                <label><i class="fas fa-columns"></i> Layout</label>
                                <div class="layout-options">
                                    <div class="layout-option active" data-layout="single">
                                        <i class="fas fa-file-alt"></i>
                                        <span>Single Column</span>
                                    </div>
                                    <div class="layout-option" data-layout="double">
                                        <i class="fas fa-columns"></i>
                                        <span>Two Column</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="form-actions">
                        <button class="btn-secondary" id="reset-form">
                            <i class="fas fa-redo"></i> Reset All
                        </button>
                        <button class="btn-primary" id="generate-resume">
                            <i class="fas fa-file-pdf"></i> Generate & Download PDF
                        </button>
                    </div>
                </div>

                <!-- Live Preview Section -->
                <div class="preview-section">
                    <div class="preview-header">
                        <h3><i class="fas fa-eye"></i> Live Preview</h3>
                        <div class="preview-actions">
                            <button class="btn-icon" id="zoom-in"><i class="fas fa-search-plus"></i></button>
                            <button class="btn-icon" id="zoom-out"><i class="fas fa-search-minus"></i></button>
                            <button class="btn-icon" id="toggle-preview"><i class="fas fa-expand"></i></button>
                        </div>
                    </div>
                    <div class="preview-container">
                        <div class="resume-preview" id="resume-preview">
                            <!-- Resume preview will be rendered here -->
                        </div>
                    </div>
                    <div class="preview-stats">
                        <div class="stat">
                            <i class="fas fa-file-word"></i>
                            <span id="word-count">0</span> words
                        </div>
                        <div class="stat">
                            <i class="fas fa-bullseye"></i>
                            <span id="ats-score">85</span> ATS Score
                        </div>
                        <div class="stat">
                            <i class="fas fa-clock"></i>
                            <span>Auto-saved</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Ad Modal -->
    <div class="modal" id="ad-modal">
        <div class="modal-content">
            <div class="modal-header">
                <h3>Unlock Premium Template</h3>
                <button class="modal-close">&times;</button>
            </div>
            <div class="modal-body">
                <div class="ad-container">
                    <div class="ad-content">
                        <i class="fas fa-ad"></i>
                        <h4>Watch a Short Ad to Continue</h4>
                        <p>Support us by watching a 30-second ad to unlock premium templates.</p>
                        <div class="ad-countdown">
                            <div class="countdown-circle">
                                <span id="countdown">30</span>s
                            </div>
                            <p>Ad will play automatically</p>
                        </div>
                        <div class="ad-placeholder">
                            <div class="ad-video-placeholder">
                                <div class="play-button">
                                    <i class="fas fa-play"></i>
                                </div>
                                <p>Advertisement Video</p>
                            </div>
                        </div>
                        <div class="ad-benefits">
                            <p><i class="fas fa-check-circle"></i> Unlock premium template</p>
                            <p><i class="fas fa-check-circle"></i> Support free service</p>
                            <p><i class="fas fa-check-circle"></i> No payment required</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="modal-footer">
                <button class="btn-secondary" id="skip-ad">Skip Ad (Use Credit)</button>
                <button class="btn-primary" id="watch-ad">Watch Ad to Unlock</button>
            </div>
        </div>
    </div>

    <!-- Success Modal -->
    <div class="modal" id="success-modal">
        <div class="modal-content success-modal">
            <div class="success-icon">
                <i class="fas fa-check-circle"></i>
            </div>
            <h3>Resume Created Successfully!</h3>
            <p>Your professional resume is ready to download.</p>
            <div class="success-actions">
                <button class="btn-secondary" id="edit-again">
                    <i class="fas fa-edit"></i> Edit Again
                </button>
                <button class="btn-primary" id="download-pdf">
                    <i class="fas fa-download"></i> Download PDF
                </button>
                <button class="btn-success" id="share-resume">
                    <i class="fas fa-share-alt"></i> Share
                </button>
            </div>
            <div class="success-tips">
                <h4><i class="fas fa-lightbulb"></i> Pro Tips:</h4>
                <ul>
                    <li>Save your resume with filename: <strong>YourName_Resume.pdf</strong></li>
                    <li>Customize for each job application</li>
                    <li>Keep it to 1-2 pages maximum</li>
                </ul>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <div class="logo">
                        <i class="fas fa-file-alt"></i>
                        <h2>Resume Creator</h2>
                    </div>
                    <p>Creating professional resumes for the Indian job market since 2024.</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-linkedin"></i></a>
                        <a href="#"><i class="fab fa-github"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                    </div>
                </div>
                <div class="footer-section">
                    <h3>Quick Links</h3>
                    <a href="#templates">Templates</a>
                    <a href="#builder">Resume Builder</a>
                    <a href="#">Examples</a>
                    <a href="#">Tips & Guides</a>
                </div>
                <div class="footer-section">
                    <h3>Resources</h3>
                    <a href="#">ATS Guidelines</a>
                    <a href="#">Cover Letter Builder</a>
                    <a href="#">Interview Prep</a>
                    <a href="#">Career Blog</a>
                </div>
                <div class="footer-section">
                    <h3>Legal</h3>
                    <a href="#">Privacy Policy</a>
                    <a href="#">Terms of Service</a>
                    <a href="#">Cookie Policy</a>
                    <a href="#">Contact Us</a>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; 2024 Resume Creator. All rights reserved. | Made with <i class="fas fa-heart"></i> for Indian job seekers</p>
                <p>Free to use • Premium templates via ads • No hidden charges</p>
            </div>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html>
