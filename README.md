<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Badagala Shyam Prasad - Infographic CV</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;800&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f0f4f8;
            color: #003F5C;
        }
        .chart-container {
            position: relative;
            margin-left: auto;
            margin-right: auto;
            height: 320px;
            width: 100%;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 400px;
            }
        }
        .timeline {
            position: relative;
            padding: 2rem 0;
        }
        .timeline::before {
            content: '';
            position: absolute;
            top: 0;
            left: 1.5rem;
            height: 100%;
            width: 4px;
            background: #665191;
            border-radius: 2px;
        }
        .timeline-item {
            position: relative;
            margin-bottom: 2rem;
            padding-left: 3.5rem;
        }
        .timeline-dot {
            position: absolute;
            left: calc(1.5rem - 0.625rem + 2px);
            top: 0.25rem;
            height: 1.25rem;
            width: 1.25rem;
            background: #D45087;
            border: 3px solid #f0f4f8;
            border-radius: 50%;
        }
        .card {
            background-color: white;
            border-radius: 0.75rem;
            box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -2px rgb(0 0 0 / 0.1);
        }
    </style>
</head>
<body class="antialiased">

    <div class="container mx-auto p-4 md:p-8 max-w-6xl">
        
        <header class="text-center p-8 rounded-lg bg-white shadow-lg mb-12">
            <h1 class="text-4xl md:text-5xl font-extrabold text-[#003F5C]">Badagala Shyam Prasad</h1>
            <p class="text-xl md:text-2xl font-medium text-[#665191] mt-2">Aspiring Software Developer</p>
            <div class="flex justify-center items-center space-x-6 mt-6 text-sm md:text-base">
                <span class="text-[#2F4B7C]">📞 9346829181</span>
                <span class="text-[#2F4B7C]">📧 shyambadagala@gmail.com</span>
                <span class="text-[#2F4B7C]">📍 Hyderabad, India</span>
            </div>
        </header>

        <main class="space-y-12">

            <section id="summary" class="card p-6 md:p-8">
                <h2 class="text-3xl font-bold text-center mb-6 text-[#A05195]">Profile Summary</h2>
                <p class="text-center text-lg max-w-3xl mx-auto text-[#2F4B7C]">
                    A motivated and curious B.Tech Computer Science student with a passion for learning, building, and collaborating. Known for being an explorer and team worker, I am actively improving my programming skills and pursuing hands-on experience through real-world projects. I am seeking opportunities where I can be productive, contribute to impactful work, and grow within the tech industry.
                </p>
            </section>
            
            <section id="skills" class="card p-6 md:p-8">
                <h2 class="text-3xl font-bold text-center mb-2 text-[#A05195]">Technical Skillset</h2>
                <p class="text-center text-md max-w-2xl mx-auto mb-8 text-[#2F4B7C]">This chart visualizes my current confidence and proficiency across key technical domains. I am a dedicated learner, continuously working to deepen and broaden this skillset.</p>
                <div class="chart-container max-w-3xl">
                    <canvas id="skillsChart"></canvas>
                </div>
            </section>
            
            <section id="strengths">
                 <h2 class="text-3xl font-bold text-center mb-8 text-[#A05195]">Core Strengths</h2>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                    <div class="card p-6 text-center">
                        <h3 class="text-xl font-bold mb-4 text-[#D45087]">Explorer Mindset</h3>
                        <div class="chart-container h-48 w-48">
                            <canvas id="explorerChart"></canvas>
                        </div>
                        <p class="mt-4 text-sm text-[#2F4B7C]">Driven by curiosity to explore new technologies and solve complex problems.</p>
                    </div>
                    <div class="card p-6 text-center">
                        <h3 class="text-xl font-bold mb-4 text-[#F95D6A]">Team Collaboration</h3>
                        <div class="chart-container h-48 w-48">
                            <canvas id="teamChart"></canvas>
                        </div>
                        <p class="mt-4 text-sm text-[#2F4B7C]">Thrives in team environments, valuing communication and shared goals.</p>
                    </div>
                    <div class="card p-6 text-center">
                        <h3 class="text-xl font-bold mb-4 text-[#FF7C43]">Eagerness to Learn</h3>
                         <div class="chart-container h-48 w-48">
                            <canvas id="learnChart"></canvas>
                        </div>
                        <p class="mt-4 text-sm text-[#2F4B7C]">A proactive and fast learner, committed to continuous personal and professional growth.</p>
                    </div>
                </div>
            </section>

            <section id="education" class="card p-6 md:p-8">
                <h2 class="text-3xl font-bold text-center mb-8 text-[#A05195]">Educational Journey</h2>
                <div class="timeline max-w-3xl mx-auto">
                    <div class="timeline-item">
                        <div class="timeline-dot"></div>
                        <h3 class="text-xl font-bold text-[#665191]">B.Tech in Computer Science Engineering</h3>
                        <p class="font-medium text-[#2F4B7C]">Sri Indu College, Sheriguda (IBP Campus)</p>
                        <p class="text-sm text-gray-500">Current</p>
                    </div>
                    <div class="timeline-item">
                        <div class="timeline-dot"></div>
                        <h3 class="text-xl font-bold text-[#665191]">Intermediate (Class 11–12)</h3>
                        <p class="font-medium text-[#2F4B7C]">Sri Viswa Junior College, Hyderabad</p>
                    </div>
                    <div class="timeline-item">
                        <div class="timeline-dot"></div>
                        <h3 class="text-xl font-bold text-[#665191]">Schooling (Class 6-10)</h3>
                        <p class="font-medium text-[#2F4B7C]">KKR Gowtham, Vizag & Hyderabad</p>
                    </div>
                     <div class="timeline-item">
                        <div class="timeline-dot"></div>
                        <h3 class="text-xl font-bold text-[#665191]">Primary Schooling (Class 1-5)</h3>
                        <p class="font-medium text-[#2F4B7C]">NRI School & St. Paul’s School</p>
                    </div>
                </div>
            </section>

            <section id="projects" class="card p-6 md:p-8">
                <h2 class="text-3xl font-bold text-center mb-8 text-[#A05195]">Project Spotlight</h2>
                <div class="max-w-3xl mx-auto p-6 rounded-lg border-2 border-[#D45087]">
                     <h3 class="text-2xl font-bold text-[#D45087]">Netflix Clone</h3>
                     <p class="mt-4 text-lg text-[#2F4B7C]">
                        I developed a responsive clone of the Netflix UI using HTML, CSS, and JavaScript. This project was a practical exercise in modern front-end development, focusing on creating a component-based structure, ensuring responsive design across devices, and implementing basic routing. It significantly enhanced my understanding of UI/UX principles and web development best practices.
                     </p>
                </div>
            </section>

            <section id="hobbies" class="card p-6 md:p-8">
                <h2 class="text-3xl font-bold text-center mb-6 text-[#A05195]">Hobbies & Interests</h2>
                <div class="flex justify-center items-center space-x-8 md:space-x-16">
                    <div class="text-center">
                        <span class="text-6xl">📚</span>
                        <p class="mt-2 text-lg font-medium text-[#2F4B7C]">Reading Books</p>
                    </div>
                    <div class="text-center">
                        <span class="text-6xl">💪</span>
                        <p class="mt-2 text-lg font-medium text-[#2F4B7C]">Gym & Fitness</p>
                    </div>
                </div>
            </section>
        </main>

    </div>

    <script>
        const tooltipTitleCallback = (tooltipItems) => {
            const item = tooltipItems[0];
            let label = item.chart.data.labels[item.dataIndex];
            if (Array.isArray(label)) {
                return label.join(' ');
            }
            return label;
        };
        
        const commonTooltipOptions = {
            plugins: {
                tooltip: {
                    callbacks: {
                        title: tooltipTitleCallback
                    },
                    backgroundColor: '#003F5C',
                    titleFont: { size: 14 },
                    bodyFont: { size: 12 },
                    padding: 10,
                    cornerRadius: 4,
                }
            }
        };

        const skillsCtx = document.getElementById('skillsChart').getContext('2d');
        new Chart(skillsCtx, {
            type: 'bar',
            data: {
                labels: [
                    ['Data Structures', '& Algorithms'], 
                    'C++', 
                    'C', 
                    'HTML/CSS/JS', 
                    ['AI Prompt', 'Engineering']
                ],
                datasets: [{
                    label: 'Proficiency',
                    data: [75, 80, 70, 85, 65],
                    backgroundColor: ['#665191', '#A05195', '#D45087', '#F95D6A', '#FF7C43'],
                    borderColor: '#fff',
                    borderWidth: 2,
                    borderRadius: 4
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                indexAxis: 'y',
                ...commonTooltipOptions,
                scales: {
                    x: {
                        beginAtZero: true,
                        max: 100,
                        grid: {
                            color: '#e0e0e020'
                        },
                        ticks: {
                            color: '#003F5C'
                        }
                    },
                    y: {
                         grid: {
                            display: false
                        },
                        ticks: {
                            color: '#003F5C',
                            font: {
                                weight: 'bold'
                            }
                        }
                    }
                },
                plugins: {
                    ...commonTooltipOptions.plugins,
                    legend: {
                        display: false
                    }
                }
            }
        });

        function createStrengthChart(canvasId, data, color) {
            const ctx = document.getElementById(canvasId).getContext('2d');
            new Chart(ctx, {
                type: 'doughnut',
                data: {
                    labels: ['Strength', ''],
                    datasets: [{
                        data: data,
                        backgroundColor: [color, '#e0e6f0'],
                        borderColor: '#ffffff',
                        borderWidth: 4,
                        hoverOffset: 4
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    cutout: '75%',
                    plugins: {
                        legend: {
                            display: false
                        },
                        tooltip: {
                           enabled: false
                        }
                    }
                }
            });
        }

        createStrengthChart('explorerChart', [90, 10], '#D45087');
        createStrengthChart('teamChart', [95, 5], '#F95D6A');
        createStrengthChart('learnChart', [98, 2], '#FF7C43');

    </script>
</body>
</html>
