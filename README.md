# BCT_SUBHO
Here's the complete enhanced project with your name **Subhodwip Mahato** and internship details integrated:

## index.html (Complete with your details)
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>StudentHub - Student Management System | Subhodwip Mahato</title>
    
    <!-- Bootstrap 5 CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary shadow-sm fixed-top">
        <div class="container">
            <a class="navbar-brand fw-bold fs-4" href="index.html">
                <i class="fas fa-graduation-cap me-2"></i>
                StudentHub
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link active" href="index.html"><i class="fas fa-home me-1"></i>Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#about" data-bs-toggle="modal"><i class="fas fa-user me-1"></i>About Me</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#project" data-bs-toggle="modal"><i class="fas fa-code me-1"></i>Project</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#contact" data-bs-toggle="modal"><i class="fas fa-envelope me-1"></i>Contact</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Main Content -->
    <main class="main-content">
        <!-- Hero Section -->
        <section class="hero-section py-5 bg-gradient-primary">
            <div class="container">
                <div class="row align-items-center min-vh-70">
                    <div class="col-lg-6">
                        <div class="animate__animated animate__fadeInUp">
                            <h1 class="display-4 fw-bold text-white mb-3">
                                StudentHub
                            </h1>
                            <h2 class="h3 fw-bold text-white mb-4 opacity-90">
                                Advanced Student Management System
                            </h2>
                            <p class="lead text-white mb-4">
                                Built by <span class="text-warning fw-bold">Subhodwip Mahato</span>
                            </p>
                            <p class="text-white-50 mb-4 fs-6">
                                Full-stack web application with CRUD operations, real-time search, and modern UI/UX
                            </p>
                            <div class="animate__animated animate__fadeInUp animate__delay-1s">
                                <button class="btn btn-warning btn-lg me-3 shadow-lg" onclick="showForm()">
                                    <i class="fas fa-plus me-2"></i>Add Student
                                </button>
                                <button class="btn btn-outline-light btn-lg shadow-lg" onclick="searchStudents()">
                                    <i class="fas fa-search me-2"></i>Search Students
                                </button>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-6 text-center animate__animated animate__fadeInRight animate__delay-1s">
                        <div class="position-relative">
                            <img src="https://images.unsplash.com/photo-1523050854058-8df90110c9f1?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" 
                                 alt="Student Management" class="img-fluid rounded-4 shadow-lg hero-img">
                            <div class="position-absolute top-0 end-0 bg-warning rounded-circle p-3 shadow-lg">
                                <i class="fas fa-chart-line fa-2x text-dark"></i>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Developer Badge -->
        <section class="py-4 bg-white">
            <div class="container">
                <div class="row justify-content-center">
                    <div class="col-lg-8 text-center">
                        <div class="developer-badge bg-gradient-primary text-white p-4 rounded-4 shadow-lg">
                            <div class="row align-items-center">
                                <div class="col-md-3 text-center mb-3 mb-md-0">
                                    <img src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1974&q=80" 
                                         alt="Subhodwip Mahato" class="rounded-circle shadow-lg" style="width: 120px; height: 120px; object-fit: cover;">
                                </div>
                                <div class="col-md-9">
                                    <h3 class="fw-bold mb-2">Subhodwip Mahato</h3>
                                    <p class="lead mb-2">Full-Stack Developer</p>
                                    <div class="d-flex flex-wrap gap-2 justify-content-center justify-content-md-start">
                                        <span class="badge bg-success">
                                            <i class="fas fa-laptop-code me-1"></i>App Development
                                        </span>
                                        <span class="badge bg-info">
                                            <i class="fas fa-shield-alt me-1"></i>Cyber Security
                                        </span>
                                        <span class="badge bg-warning text-dark">
                                            <i class="fas fa-certificate me-1"></i>Euphoria GenX Intern
                                        </span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Stats Cards -->
        <section class="stats-section py-5 bg-light">
            <div class="container">
                <div class="row g-4 text-center">
                    <div class="col-md-3 col-sm-6">
                        <div class="stat-card bg-primary text-white p-4 rounded-4 shadow-lg hover-lift">
                            <i class="fas fa-users fa-3x mb-3"></i>
                            <h3 id="totalStudents" class="fw-bold fs-1">0</h3>
                            <p class="mb-0">Total Students</p>
                        </div>
                    </div>
                    <div class="col-md-3 col-sm-6">
                        <div class="stat-card bg-success text-white p-4 rounded-4 shadow-lg hover-lift">
                            <i class="fas fa-book fa-3x mb-3"></i>
                            <h3 id="totalCourses" class="fw-bold fs-1">0</h3>
                            <p class="mb-0">Courses</p>
                        </div>
                    </div>
                    <div class="col-md-3 col-sm-6">
                        <div class="stat-card bg-warning text-dark p-4 rounded-4 shadow-lg hover-lift">
                            <i class="fas fa-star fa-3x mb-3"></i>
                            <h3 id="topStudents" class="fw-bold fs-1">0</h3>
                            <p class="mb-0">Top Performers</p>
                        </div>
                    </div>
                    <div class="col-md-3 col-sm-6">
                        <div class="stat-card bg-info text-white p-4 rounded-4 shadow-lg hover-lift">
                            <i class="fas fa-chart-line fa-3x mb-3"></i>
                            <h3 class="fw-bold fs-1">100%</h3>
                            <p class="mb-0">Success Rate</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Search & Filter Section -->
        <section class="py-5">
            <div class="container">
                <div class="row justify-content-center">
                    <div class="col-lg-10">
                        <div class="card shadow-xl border-0 rounded-5 overflow-hidden">
                            <div class="card-header bg-gradient-primary text-white py-4">
                                <div class="row align-items-center">
                                    <div class="col-md-6">
                                        <h3 class="mb-0 fw-bold">
                                            <i class="fas fa-list me-2"></i>
                                            Student Directory
                                        </h3>
                                        <small class="text-white-50">Manage your students efficiently</small>
                                    </div>
                                    <div class="col-md-6 text-md-end mt-3 mt-md-0">
                                        <div class="input-group input-group-lg">
                                            <span class="input-group-text bg-white border-end-0 text-muted">
                                                <i class="fas fa-search"></i>
                                            </span>
                                            <input type="text" id="searchInput" class="form-control border-start-0 shadow-none" 
                                                   placeholder="🔍 Search by name, email, course or grade..." onkeyup="filterStudents()">
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="card-body p-0">
                                <!-- Add Student Form -->
                                <div id="addForm" class="p-5 bg-light border-bottom" style="display: none;">
                                    <div class="row align-items-center mb-4">
                                        <div class="col">
                                            <h4 class="fw-bold mb-0 text-primary">
                                                <i class="fas fa-user-plus me-2"></i>New Student Registration
                                            </h4>
                                        </div>
                                        <div class="col-auto">
                                            <button class="btn btn-outline-secondary" onclick="hideForm()">
                                                <i class="fas fa-times"></i> Cancel
                                            </button>
                                        </div>
                                    </div>
                                    <form id="studentForm">
                                        <div class="row g-4">
                                            <div class="col-md-6">
                                                <label class="form-label fw-semibold text-dark">👤 Full Name</label>
                                                <input type="text" class="form-control form-control-lg shadow-sm" id="name" required>
                                            </div>
                                            <div class="col-md-6">
                                                <label class="form-label fw-semibold text-dark">📧 Email</label>
                                                <input type="email" class="form-control form-control-lg shadow-sm" id="email" required>
                                            </div>
                                            <div class="col-md-6">
                                                <label class="form-label fw-semibold text-dark">🎂 Age</label>
                                                <input type="number" class="form-control form-control-lg shadow-sm" id="age" min="16" max="80" required>
                                            </div>
                                            <div class="col-md-6">
                                                <label class="form-label fw-semibold text-dark">📚 Course</label>
                                                <select class="form-select form-select-lg shadow-sm" id="course" required>
                                                    <option value="">Choose Course</option>
                                                    <option value="Computer Science">💻 Computer Science</option>
                                                    <option value="Business Admin">💼 Business Administration</option>
                                                    <option value="Engineering">🔧 Engineering</option>
                                                    <option value="Medicine">🏥 Medicine</option>
                                                    <option value="Law">⚖️ Law</option>
                                                    <option value="Arts">🎨 Arts & Humanities</option>
                                                </select>
                                            </div>
                                            <div class="col-md-6">
                                                <label class="form-label fw-semibold text-dark">⭐ Grade (%)</label>
                                                <input type="number" min="0" max="100" class="form-control form-control-lg shadow-sm" id="grade" required>
                                            </div>
                                            <div class="col-12">
                                                <button type="submit" class="btn btn-primary btn-lg px-5 shadow-lg">
                                                    <i class="fas fa-save me-2"></i>Save Student
                                                </button>
                                            </div>
                                        </div>
                                    </form>
                                </div>

                                <!-- Students Table -->
                                <div id="studentsTable" class="p-5">
                                    <div class="table-responsive">
                                        <table class="table table-hover align-middle mb-0">
                                            <thead class="table-dark">
                                                <tr>
                                                    <th width="60"><i class="fas fa-hashtag"></i></th>
                                                    <th><i class="fas fa-user"></i> Name</th>
                                                    <th><i class="fas fa-envelope"></i> Email</th>
                                                    <th><i class="fas fa-calendar"></i> Age</th>
                                                    <th><i class="fas fa-book"></i> Course</th>
                                                    <th><i class="fas fa-star"></i> Grade</th>
                                                    <th width="150"><i class="fas fa-cogs"></i> Actions</th>
                                                </tr>
                                            </thead>
                                            <tbody id="studentsBody">
                                            </tbody>
                                        </table>
                                    </div>
                                    <div id="noStudents" class="text-center py-5 d-none">
                                        <i class="fas fa-users fa-5x text-muted mb-4 opacity-50"></i>
                                        <h4 class="text-muted fw-bold">No students found</h4>
                                        <p class="text-muted lead">Start by adding your first student!</p>
                                        <button class="btn btn-primary btn-lg px-5 shadow-lg" onclick="showForm()">
                                            <i class="fas fa-plus-circle me-2"></i>Add First Student
                                        </button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-dark text-white py-5 mt-auto">
        <div class="container">
            <div class="row">
                <div class="col-lg-4 mb-4">
                    <h5 class="fw-bold mb-3">
                        <i class="fas fa-graduation-cap me-2 text-warning"></i>
                        StudentHub
                    </h5>
                    <p class="text-light-50">Advanced Student Management System developed by Subhodwip Mahato</p>
                </div>
                <div class="col-lg-4 mb-4">
                    <h6 class="fw-bold mb-3 text-light">Developer</h6>
                    <p class="text-light-50 mb-1">Subhodwip Mahato</p>
                    <p class="text-light-50 small mb-0">
                        <i class="fas fa-briefcase me-1"></i>Internships: App Development & Cyber Security<br>
                        <i class="fas fa-building me-1"></i>Euphoria GenX
                    </p>
                </div>
                <div class="col-lg-4 mb-4">
                    <h6 class="fw-bold mb-3">Quick Links</h6>
                    <ul class="list-unstyled">
                        <li><a href="#about" class="text-light-50 text-decoration-none hover-white" data-bs-toggle="modal"><i class="fas fa-user me-2"></i>About Developer</a></li>
                        <li><a href="#project" class="text-light-50 text-decoration-none hover-white" data-bs-toggle="modal"><i class="fas fa-code me-2"></i>Project Details</a></li>
                        <li><a href="#contact" class="text-light-50 text-decoration-none hover-white" data-bs-toggle="modal"><i class="fas fa-envelope me-2"></i>Contact</a></li>
                    </ul>
                </div>
            </div>
            <hr class="my-4 opacity-25">
            <div class="text-center">
                <p class="mb-0 text-light-50">
                    &copy; 2024 <strong>StudentHub</strong> by <strong>Subhodwip Mahato</strong> | 
                    Made with <i class="fas fa-heart text-danger"></i> during Euphoria GenX Internship
                </p>
            </div>
        </div>
    </footer>

    <!-- About Developer Modal -->
    <div class="modal fade" id="about" tabindex="-1">
        <div class="modal-dialog modal-lg modal-dialog-centered">
            <div class="modal-content rounded-4 shadow-xl border-0">
                <div class="modal-header border-0 bg-gradient-primary text-white rounded-top-4">
                    <div class="d-flex align-items-center">
                        <img src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-4.0.3&auto=format&fit=crop&w=200&q=80" 
                             alt="Subhodwip Mahato" class="rounded-circle me-3" style="width: 60px; height: 60px;">
                        <div>
                            <h5 class="modal-title fw-bold mb-0">Subhodwip Mahato</h5>
                            <small>Full-Stack Developer</small>
                        </div>
                    </div>
                    <button type="button" class="btn-close btn-close-white" data-bs-dismiss="modal"></button>
                </div>
                <div class="modal-body p-4">
                    <div class="row">
                        <div class="col-md-4 text-center mb-4">
                            <div class="p-3 bg-light rounded-3">
                                <i class="fas fa-laptop-code fa-3x text-primary mb-3"></i>
                                <h6 class="fw-bold">App Development</h6>
                                <p class="text-muted small mb-0">Euphoria GenX Internship</p>
                            </div>
                        </div>
                        <div class="col-md-4 text-center mb-4">
                            <div class="p-3 bg-light rounded-3">
                                <i class="fas fa-shield-alt fa-3x text-success mb-3"></i>
                                <h6 class="fw-bold">Cyber Security</h6>
                                <
<!DOCTYPE html>
<html>
<head>

<title>Django Project</title>

<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">

<style>
body{
background-color:#f8f9fa;
}

footer{
position:fixed;
bottom:0;
width:100%;
}
</style>

</head>

<body>

<!-- Navbar -->

<nav class="navbar navbar-expand-lg navbar-dark bg-primary">
<div class="container">

<a class="navbar-brand" href="/">Django Project</a>

<ul class="navbar-nav ms-auto">

<li class="nav-item">
<a class="nav-link" href="/">Home</a>
</li>

<li class="nav-item">
<a class="nav-link" href="/about">About</a>
</li>

<li class="nav-item">
<a class="nav-link" href="/contact">Contact</a>
</li>

</ul>

</div>
</nav>

<div class="container mt-4">

{% block content %}

{% endblock %}

</div>

<!-- Footer -->

<footer class="bg-dark text-white text-center p-3">
Subhodwip Mahato | Roll 32 | Django Project
</footer>

</body>

</html>
{% extends 'base.html' %}

{% block content %}

<div class="card p-4 shadow">

<h2>About Project</h2>

<hr>

<p>This project is created using Django Framework.</p>

<h4>Student Details</h4>

<ul>
<li>Name : Subhodwip Mahato</li>
<li>Roll No : 32</li>
<li>Department : CSE</li>
<li>Section : C</li>
</ul>

</div>

{% endblock %}
{% extends 'base.html' %}

{% block content %}

<div class="card p-4 shadow">

<h2>Contact Us</h2>

<form>

<div class="mb-3">
<label>Name</label>
<input type="text" class="form-control">
</div>

<div class="mb-3">
<label>Email</label>
<input type="email" class="form-control">
</div>

<div class="mb-3">
<label>Message</label>
<textarea class="form-control"></textarea>
</div>

<button class="btn btn-primary">Submit</button>

</form>

</div>

{% endblock %}
from django.shortcuts import render

def home(request):
    return render(request,'home.html')

def about(request):
    return render(request,'about.html')

def contact(request):
    return render(request,'contact.html')
from django.urls import path
from . import views

urlpatterns = [

path('',views.home,name='home'),
path('about/',views.about,name='about'),
path('contact/',views.contact,name='contact'),

]
python manage.py runserver
