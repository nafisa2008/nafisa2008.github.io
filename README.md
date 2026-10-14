<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>ApnaSaath | Care, Safety & Companionship</title>

    <style>
        /* GENERAL STYLING */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background-color: #fffdf6;
            color: #26382e;
            line-height: 1.6;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        img {
            max-width: 100%;
            display: block;
        }

        section {
            padding: 75px 8%;
            scroll-margin-top: 85px;
        }

        h1, h2, h3 {
            line-height: 1.25;
        }

        h2 {
            font-size: 2.2rem;
            margin-bottom: 18px;
        }

        p {
            color: #58645c;
        }

        .section-heading {
            text-align: center;
            max-width: 700px;
            margin: 0 auto 45px;
        }

        .section-heading p {
            margin-top: 12px;
        }

        .highlight {
            color: #39845b;
        }

        .btn {
            display: inline-block;
            padding: 13px 25px;
            background-color: #39845b;
            color: white;
            border-radius: 7px;
            font-weight: bold;
            border: 2px solid #39845b;
            transition: 0.3s;
            cursor: pointer;
            font-size: 1rem;
        }

        .btn:hover {
            background-color: #286642;
            border-color: #286642;
            transform: translateY(-2px);
        }

        .btn-outline {
            background-color: transparent;
            color: #39845b;
            margin-left: 10px;
        }

        .btn-outline:hover {
            color: white;
        }

        /* HEADER */

        header {
            width: 100%;
            background-color: #fffdf6;
            padding: 17px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 25px;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 12px rgba(0, 0, 0, 0.07);
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: #39845b;
            white-space: nowrap;
        }

        .logo span {
            color: #d89b49;
        }

        nav {
            display: flex;
            align-items: center;
            justify-content: center;
            flex-wrap: wrap;
            gap: 22px;
        }

        nav a {
            font-size: 0.95rem;
            font-weight: 600;
            color: #34483a;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #39845b;
        }

        /* HERO SECTION */

        .hero {
            min-height: 620px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            gap: 45px;
            background: linear-gradient(135deg, #f2f7e9, #fff8e9);
            padding-top: 85px;
            padding-bottom: 85px;
        }

        .hero-content {
            flex: 1;
        }

        .hero-label {
            display: inline-block;
            background-color: #e0edda;
            color: #286642;
            padding: 8px 15px;
            border-radius: 30px;
            font-size: 0.9rem;
            font-weight: bold;
            margin-bottom: 22px;
        }

        .hero h1 {
            font-size: clamp(2.5rem, 5vw, 4rem);
            margin-bottom: 22px;
            color: #26382e;
        }

        .hero-content p {
            font-size: 1.1rem;
            max-width: 570px;
            margin-bottom: 30px;
        }

        .hero-image {
            flex: 1;
            min-height: 350px;
            border-radius: 25px;
            background: linear-gradient(145deg, #dcebd4, #f5dfb7);
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 35px;
        }

        .hero-illustration {
            max-width: 400px;
        }

        .hero-illustration .emoji {
            font-size: 7rem;
            margin-bottom: 20px;
        }

        .hero-illustration h3 {
            font-size: 1.7rem;
            color: #286642;
            margin-bottom: 12px;
        }

        .hero-illustration p {
            color: #526552;
        }

        /* ABOUT SECTION */

        .about {
            display: flex;
            align-items: center;
            gap: 55px;
        }

        .about-image {
            flex: 1;
            min-height: 330px;
            background-color: #e8f0df;
            border-radius: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 30px;
        }

        .about-image .emoji {
            font-size: 6rem;
            margin-bottom: 15px;
        }

        .about-content {
            flex: 1;
        }

        .about-content h2 {
            margin-bottom: 20px;
        }

        .about-content p {
            margin-bottom: 16px;
        }

        .about-points {
            list-style: none;
            margin-top: 20px;
        }

        .about-points li {
            margin-bottom: 12px;
            color: #435548;
        }

        .about-points li::before {
            content: "✓";
            color: #39845b;
            font-weight: bold;
            margin-right: 10px;
        }

        /* SERVICES SECTION */

        .services {
            background-color: #f5f7ef;
        }

        .service-grid {
            display: grid;
            grid-template-columns: repeat(3, minmax(0, 1fr));
            gap: 25px;
        }

        .service-card {
            background-color: white;
            padding: 30px 25px;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(36, 67, 43, 0.06);
            border: 1px solid #e7ebdf;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .service-card:hover {
            transform: translateY(-6px);
            box-shadow: 0 10px 25px rgba(36, 67, 43, 0.12);
        }

        .service-icon {
            width: 60px;
            height: 60px;
            background-color: #e7f1df;
            border-radius: 14px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.9rem;
            margin-bottom: 20px;
        }

        .service-card h3 {
            font-size: 1.25rem;
            margin-bottom: 12px;
        }

        .service-card p {
            font-size: 0.96rem;
        }

        /* WHY APNASAATH */

        .why-us {
            background-color: #fffdf6;
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(3, minmax(0, 1fr));
            gap: 25px;
        }

        .feature-card {
            text-align: center;
            padding: 28px 22px;
            border-radius: 15px;
            background-color: #f8f5e9;
        }

        .feature-card .icon {
            font-size: 2.7rem;
            margin-bottom: 15px;
        }

        .feature-card h3 {
            margin-bottom: 12px;
        }

        /* SAFETY SECTION */

        .safety {
            background-color: #eaf2e3;
        }

        .safety-container {
            display: flex;
            align-items: center;
            justify-content: space-between;
            gap: 50px;
        }

        .safety-content {
            flex: 1;
        }

        .safety-content p {
            margin: 15px 0;
        }

        .safety-list {
            list-style: none;
            margin-top: 25px;
        }

        .safety-list li {
            background-color: rgba(255, 255, 255, 0.75);
            padding: 14px 18px;
            border-radius: 8px;
            margin-bottom: 12px;
        }

        .safety-list strong {
            color: #286642;
        }

        .safety-visual {
            flex: 0.8;
            min-height: 300px;
            border-radius: 20px;
            background-color: #d6e7ce;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 30px;
        }

        .safety-visual .emoji {
            font-size: 6rem;
            margin-bottom: 20px;
        }

        .safety-visual h3 {
            color: #286642;
            font-size: 1.5rem;
        }

        /* HOW IT WORKS */

        .steps-grid {
            display: grid;
            grid-template-columns: repeat(3, minmax(0, 1fr));
            gap: 25px;
        }

        .step-card {
            padding: 30px 25px;
            border: 1px solid #e4e9dd;
            border-radius: 15px;
            background-color: white;
            text-align: center;
        }

        .step-number {
            width: 55px;
            height: 55px;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0 auto 20px;
            border-radius: 50%;
            background-color: #39845b;
            color: white;
            font-size: 1.3rem;
            font-weight: bold;
        }

        .step-card h3 {
            margin-bottom: 12px;
        }

        /* COMMUNITY SECTION */

        .community {
            background-color: #f5f7ef;
        }

        .community-container {
            display: flex;
            align-items: center;
            gap: 45px;
        }

        .community-content {
            flex: 1;
        }

        .community-content p {
            margin-bottom: 18px;
        }

        .community-visual {
            flex: 1;
            min-height: 300px;
            background: linear-gradient(135deg, #e5eedb, #f9e6c7);
            border-radius: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 30px;
        }

        .community-visual .emoji {
            font-size: 6rem;
            margin-bottom: 15px;
        }

        .community-visual h3 {
            color: #286642;
        }

        /* FAMILY CONNECT */

        .family {
            display: flex;
            align-items: center;
            gap: 50px;
        }

        .family-content,
        .family-visual {
            flex: 1;
        }

        .family-content p {
            margin-bottom: 16px;
        }

        .family-visual {
            min-height: 300px;
            background-color: #f8ebd5;
            border-radius: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 30px;
        }

        .family-visual .emoji {
            font-size: 6rem;
            margin-bottom
