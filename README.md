<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shivam Jal - Pure & Safe Drinking Water Supplier</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* --- CSS VARIABLES (Light Theme Default) --- */
        :root {
            --bg-primary: #ffffff;
            --bg-secondary: #f4f9fc;
            --text-primary: #2c3e50;
            --text-secondary: #5a6c7d;
            --accent: #00a8ff;
            --accent-hover: #0086cc;
            --card-bg: #ffffff;
            --shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
            --transition: all 0.3s ease;
        }

        /* --- DARK THEME VARIABLES --- */
        [data-theme="dark"] {
            --bg-primary: #121212;
            --bg-secondary: #1e1e1e;
            --text-primary: #f5f6fa;
            --text-secondary: #b8bfc6;
            --accent: #00a8ff;
            --accent-hover: #33b8ff;
            --card-bg: #1e1e1e;
            --shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
        }

        /* --- BASE STYLES --- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--bg-primary);
            color: var(--text-primary);
            transition: var(--transition);
            line-height: 1.6;
        }

        section {
            padding: 80px 10%;
        }

        .heading {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 40px;
            position: relative;
        }

        .heading::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 60px;
            height: 4px;
            background-color: var(--accent);
            border-radius: 2px;
        }

        /* --- NAVBAR --- */
        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: var(--bg-primary);
            box-shadow: var(--shadow);
            z-index: 1000;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 10%;
            transition: var(--transition);
        }

        .logo {
            font-size: 1.6rem;
            font-weight: bold;
            color: var(--accent);
            display: flex;
            align-items: center;
            gap: 10px;
            text-decoration: none;
        }

        .nav-links {
            display: flex;
            list-style: none;
            align-items: center;
            gap: 30px;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text-primary);
            font-weight: 500;
            transition: var(--transition);
        }

        .nav-links a:hover {
            color: var(--accent);
        }

        .nav-actions {
            display: flex;
            align-items: center;
            gap: 20px;
        }

        .theme-toggle {
            background: none;
            border: none;
            color: var(--text-primary);
            font-size: 1.3rem;
            cursor: pointer;
            transition: var(--transition);
        }

        .menu-btn {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--text-primary);
        }

        /* --- HOME (HERO) --- */
        #home {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: space-between;
            background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url('https://images.unsplash.com/photo-1523362628745-0c100150b504?auto=format&fit=crop&w=1920&q=80') no-repeat center center/cover;
            color: white;
            text-align: left;
        }

        .hero-content {
            max-width: 600px;
        }

        .hero-content h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            font-weight: 800;
            animation: fadeInUp 1s ease;
        }

        .hero-content p {
            font-size: 1.2rem;
            margin-bottom: 30px;
            color: #e0e0e0;
        }

        .btn {
            display: inline-block;
            padding: 12