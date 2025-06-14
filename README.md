<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="utf-8">
  <meta content="width=device-width, initial-scale=1.0" name="viewport">
  <title>AI Expert Portfolio - Clayton Gwava</title>
  <meta content="Clayton Gwava's AI Expert Portfolio showcasing modern and futuristic designs, specializing in LLM-powered systems, fine-tuning, RAG, and scalable chatbots." name="description">
  <meta content="AI, Artificial Intelligence, Portfolio, Expert, Futuristic, Machine Learning, Data Science, LLM, Generative AI, Python, Java, React, Spring Boot, Docker" name="keywords">

  <!-- Favicons -->
  <link href="assets/img/favicon.png" rel="icon">
  <link href="assets/img/apple-touch-icon.png" rel="apple-touch-icon">

  <!-- Google Fonts - Orbitron for headings, Poppins for body/nav -->
  <link href="https://fonts.googleapis.com" rel="preconnect">
  <link href="https://fonts.gstatic.com" rel="preconnect" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;500;600;700;800;900&family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

  <!-- Vendor CSS Files -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" crossorigin="anonymous">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css" rel="stylesheet">
  <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
  <link href="https://cdn.jsdelivr.net/npm/glightbox/dist/css/glightbox.min.css" rel="stylesheet">
  <link href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css" rel="stylesheet">
  <!-- Font Awesome for social icons -->
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">


  <!-- Custom Modernized CSS -->
  <style>
    /* Custom Color Palette & Fonts */
    :root {
      --background-color: #FFFFFF;
      /* Pure white background */
      --default-color: hsl(210, 20%, 20%);
      /* Dark blue-grey for general text */
      --heading-color: hsl(210, 25%, 15%);
      /* Even darker blue-grey for prominent headings */
      --accent-color: hsl(210, 100%, 45%);
      /* Vibrant Blue, primary accent color */
      --secondary-accent-color: hsl(30, 100%, 50%);
      /* Vibrant Orange, secondary accent for contrast */
      --surface-color: hsl(210, 10%, 98%);
      /* Very light blue-grey for card backgrounds */
      --contrast-color: #FFFFFF;
      /* White for text on dark/accent backgrounds */

      /* For rgba conversions from hsl, to make overlay transparent */
      --heading-color-rgb: 38, 51, 64;
      /* Approx RGB for hsl(210, 25%, 15%) */
      --background-color-rgb: 255, 255, 255;
      /* RGB for #FFFFFF */
      --default-font: 'Poppins', sans-serif;
      --heading-font: 'Orbitron', sans-serif;
      --nav-font: 'Poppins', sans-serif;
      /* Poppins for nav links */
    }

    /* Dark Mode specific variables */
    body.dark-mode {
      --background-color: hsl(210, 25%, 12%);
      /* Dark background */
      --default-color: hsl(210, 10%, 85%);
      /* Light grey for general text */
      --heading-color: hsl(210, 20%, 95%);
      /* Lighter grey for headings */
      --accent-color: hsl(210, 100%, 60%);
      /* Slightly brighter blue for dark mode */
      --secondary-accent-color: hsl(30, 100%, 65%);
      /* Slightly brighter orange for dark mode */
      --surface-color: hsl(210, 20%, 18%);
      /* Darker surface for cards/elements */


      /* Adjust rgba for dark mode */
      --heading-color-rgb: 242, 245, 247;
      /* Approx RGB for hsl(210, 20%, 95%) */
      --background-color-rgb: 30, 39, 48;
      /* Approx RGB for hsl(210, 25%, 12%) */
    }

    /* Color Presets */
    .light-background {
      background-color: hsl(210, 10%, 99%) !important;
    }

    .dark-background {
      background-color: hsl(210, 25%, 15%) !important;
      color: hsl(210, 10%, 85%) !important;
    }

    /* Smooth scroll */
    :root {
      scroll-behavior: smooth;
    }

    /*--------------------------------------------------------------
    # General Styling & Shared Classes
    --------------------------------------------------------------*/
    body {
      color: var(--default-color);
      background-color: var(--background-color);
      font-family: var(--default-font);
      overflow-x: hidden;
      padding-top: 0 !important;
      /* Ensure no default body padding from Bootstrap */
      transition: background-color 0.4s ease, color 0.4s ease;
      /* Smooth theme transition */
    }

    body.no-scroll {
      overflow: hidden;
      /* Disable scrolling when overlay is active */
    }

    a {
      color: var(--accent-color);
      text-decoration: none;
      transition: all 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
    }

    a:hover {
      color: var(--secondary-accent-color);
      text-decoration: none;
      transform: translateY(-2px);
    }

    h1,
    h2,
    h3,
    h4,
    h5,
    h6 {
      color: var(--heading-color);
      font-family: var(--heading-font);
      text-transform: uppercase;
      letter-spacing: 1.5px;
      transition: color 0.4s ease;
      /* Smooth theme transition */
    }

    p,
    span,
    li {
      transition: color 0.4s ease;
      /* Smooth theme transition for text elements */
    }

    /* PHP Email Form Messages */
    .php-email-form .error-message {
      display: none;
      background: hsl(0, 70%, 50%);
      /* Red for error messages */
      color: #ffffff;
      text-align: left;
      padding: 15px;
      margin-bottom: 24px;
      font-weight: 600;
      border-radius: 8px;
    }

    .php-email-form .sent-message {
      display: none;
      color: #ffffff;
      background: hsl(120, 60%, 40%);
      /* Green for success messages */
      text-align: center;
      padding: 15px;
      margin-bottom: 24px;
      font-weight: 600;
      border-radius: 8px;
    }

    .php-email-form .loading {
      display: none;
      background: var(--surface-color);
      text-align: center;
      padding: 15px;
      margin-bottom: 24px;
      border-radius: 8px;
    }

    .php-email-form .loading:before {
      content: "";
      display: inline-block;
      border-radius: 50%;
      width: 24px;
      height: 24px;
      margin: 0 10px -6px 0;
      border: 3px solid var(--accent-color);
      border-top-color: var(--surface-color);
      animation: php-email-form-loading 1s linear infinite;
    }

    @keyframes php-email-form-loading {
      0% {
        transform: rotate(0deg);
      }

      100% {
        transform: rotate(360deg);
      }
    }

    /*--------------------------------------------------------------
    # Header & Mobile Nav (NEW)
    --------------------------------------------------------------*/
    .header {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      padding: 20px 0;
      z-index: 1002;
      /* Above floating social and appbar */
      display: flex;
      justify-content: space-between;
      align-items: center;
      /* Adjusted background-color opacity for more transparency */
      background-color: rgba(var(--background-color-rgb), 0.05);
      /* Very light background */
      /* Increased blur for frosted glass effect */
      backdrop-filter: blur(15px);
      /* Stronger blur */
      -webkit-backdrop-filter: blur(15px);
      /* For Safari */
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
      /* Subtle shadow */
      transition: background-color 0.4s ease, box-shadow 0.4s ease, backdrop-filter 0.4s ease;
    }

    body.dark-mode .header {
      background-color: rgba(var(--background-color-rgb), 0.1);
      /* Slightly more visible in dark mode */
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
      /* Darker shadow in dark mode */
    }

    .header .logo {
      margin-left: 25px;
      color: #ffffff;
      /* White text for logo */
      font-family: var(--heading-font);
      font-size: 28px;
      font-weight: 700;
      text-decoration: none;
      position: relative;
      z-index: 1003;
      text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.5);
      /* Stronger shadow for visibility against transparent background */
      transition: color 0.4s ease, text-shadow 0.4s ease;
    }

    .header .logo span {
      color: var(--accent-color);
      transition: color 0.4s ease;
    }

    /* Main Navigation (for desktop) */
    .main-nav {
      flex-grow: 1;
      /* Allows it to take available space */
      text-align: center;
      /* Centers the ul */
      margin: 0 25px;
      /* Adjust margin to ensure it's not too wide */
    }

    .main-nav ul {
      list-style: none;
      padding: 0;
      margin: 0;
      display: inline-flex;
      /* Keeps items together while centering */
      gap: 30px;
    }

    .main-nav a {
      color: #ffffff;
      /* White text for nav links by default */
      font-family: var(--nav-font);
      font-size: 16px;
      font-weight: 500;
      text-transform: uppercase;
      transition: color 0.3s ease, transform 0.3s ease;
      position: relative;
      padding-bottom: 5px;
      text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.5);
      /* Stronger shadow for visibility */
    }

    body.dark-mode .main-nav a {
      color: var(--default-color);
      /* Lighter text in dark mode */
      text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.7);
      /* Slightly stronger shadow in dark mode */
    }

    .main-nav a:hover,
    .main-nav a.active {
      color: var(--accent-color);
      transform: translateY(-2px);
    }

    .main-nav a::after {
      content: '';
      position: absolute;
      width: 0;
      height: 2px;
      background: var(--accent-color);
      left: 50%;
      bottom: 0;
      transform: translateX(-50%);
      transition: width 0.3s ease;
    }

    .main-nav a:hover::after,
    .main-nav a.active::after {
      width: 100%;
    }

    /* Hamburger Menu for Mobile */
    .mobile-nav-toggle {
      position: fixed;
      top: 30px;
      right: 25px;
      z-index: 1005;
      background: transparent url('assets/img/hamburger-icon.svg') no-repeat center center;
      background-size: auto;
      border: none;
      font-size: 30px;
      color: orange;
      /* White icon for mobile toggle */
      cursor: pointer;
      display: none;
      /* Hidden by default, shown on mobile */
      transition: all 0.3s ease;
      text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.5);
      /* Stronger shadow for visibility */
    }

    body.dark-mode .mobile-nav-toggle {
      color: var(--default-color);
      /* Lighter icon in dark mode */
      text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.7);
    }

    .mobile-nav-toggle:hover {
      color: var(--accent-color);
    }

    .mobile-nav {
      position: fixed;
      top: 0;
      right: -100%;
      /* Start off-screen */
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.98);
      /* Near-black for maximum text contrast */
      z-index: 1002;
      transition: all 0.3s ease-in-out;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      opacity: 0;
      visibility: hidden;
      backdrop-filter: blur(25px);
      /* Increased blur for more prominence */
      -webkit-backdrop-filter: blur(25px);
      /* For Safari support */
      box-shadow: -5px 0 30px rgba(0, 0, 0, 0.5);
      /* Shadow for pop-out effect */
    }

    .mobile-nav.active {
      right: 0;
      opacity: 1;
      visibility: visible;
    }

    .mobile-nav ul {
      list-style: none;
      padding: 0;
      margin: 0;
      text-align: center;
    }

    .mobile-nav ul li {
      margin: 15px 0;
      /* Increased vertical margin for better spacing */
    }

    .mobile-nav a {
      color: #FFFFFF;
      /* Always white text for mobile nav links */
      font-family: var(--heading-font);
      font-size: 22px;
      /* Slightly larger font for better visibility */
      font-weight: 700;
      /* Bolder font for more impact */
      text-decoration: none;
      transition: color 0.3s ease;
      text-shadow: 0px 0px 10px rgba(255, 255, 255, 0.3);
      /* Stronger glow for clarity */
    }

    .mobile-nav a:hover {
      color: var(--accent-color);
      /* Keep accent color for hover */
      text-shadow: none;
      /* Remove glow on hover if it clashes with accent */
    }

    @media (max-width: 768px) {
      .main-nav {
        display: none;
        /* Hide main nav on mobile */
      }

      .mobile-nav-toggle {
        display: block;
        /* Show hamburger on mobile */
      }

      .header .logo {
        position: absolute;
        left: 25px;
        /* Keep logo on the left */
        top: 20px;
        font-size: 24px;
        /* Slightly smaller logo on mobile */
      }

      /* Hide logo when mobile nav is active */
      .mobile-nav.active+.logo-container .logo {
        display: none;
      }
    }


    /*--------------------------------------------------------------
    # Top Text Navigation (OLD - No longer used for main nav)
    --------------------------------------------------------------*/
    /* This section is retained for reference but its styles are largely superseded by .main-nav and .mobile-nav */
    .top-text-nav {
      display: none;
      /* Hidden by default, replaced by main-nav/mobile-nav */
    }


    /*--------------------------------------------------------------
    # Floating Social Only (Left)
    --------------------------------------------------------------*/
    .floating-social-only {
      position: fixed;
      left: 0;
      top: 50%;
      transform: translateY(-50%);
      z-index: 1000;
      background: rgba(var(--heading-color-rgb), 0.1);
      /* Transparent background using RGB var */
      border-radius: 0 15px 15px 0;
      overflow: hidden;
      display: flex;
      flex-direction: column;
      padding: 10px 0px;
      box-shadow: 0px 6px 25px rgba(0, 0, 0, 0.5);
      /* Even stronger shadow */
      align-items: center;
      backdrop-filter: blur(8px);
      /* Added backdrop filter */
    }

    .floating-social-only a {
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      padding: 12px;
      font-size: 28px;
      text-align: center;
      transition: background 0.3s ease, transform 0.3s ease;
      text-decoration: none;
      border-radius: 50%;
      margin: 5px 0;
      width: 50px;
      height: 50px;
      text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.4);
      /* Text shadow for visibility */
    }

    .floating-social-only a:hover {
      background: var(--accent-color);
      transform: translateX(5px) scale(1.1);
      color: var(--contrast-color);
      box-shadow: 0 0 15px var(--accent-color);
      text-shadow: none;
      /* Remove text shadow on hover */
    }

    /* Ensure icons are white within the floating social bar */
    .floating-social-only a i {
      color: white;
    }

    /* Tooltip for floating social */
    .floating-social-only a .tooltiptext {
      visibility: hidden;
      width: auto;
      background-color: rgba(var(--heading-color-rgb), 0.8);
      /* Transparent background for tooltip */
      color: #fff;
      text-align: center;
      border-radius: 6px;
      padding: 5px 10px;
      position: absolute;
      z-index: 1;
      left: 100%;
      margin-left: 10px;
      opacity: 0;
      transition: opacity 0.3s;
      font-size: 14px;
      white-space: nowrap;
      backdrop-filter: blur(5px);
      /* Blur for tooltip */
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
      /* Shadow for tooltip */
    }

    .floating-social-only a:hover .tooltiptext {
      visibility: visible;
      opacity: 1;
    }

    .floating-social-only a .tooltiptext::after {
      content: " ";
      position: absolute;
      right: 100%;
      top: 50%;
      margin-top: -5px;
      border-width: 5px;
      border-style: solid;
      border-color: transparent rgba(var(--heading-color-rgb), 0.8) transparent transparent;
    }

    /* Dark mode for floating social */
    body.dark-mode .floating-social-only {
      background: rgba(var(--surface-color), 0.1);
      /* Transparent background using surface color for dark mode */
      box-shadow: 0px 6px 25px rgba(0, 0, 0, 0.7);
      /* Even stronger shadow for dark mode */
    }

    body.dark-mode .floating-social-only a {
      color: var(--default-color);
      /* Icons in dark mode */
      text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.5);
    }

    body.dark-mode .floating-social-only a:hover {
      background: var(--accent-color);
      color: var(--contrast-color);
      box-shadow: 0 0 15px var(--accent-color);
    }

    body.dark-mode .floating-social-only a .tooltiptext {
      background-color: rgba(var(--surface-color), 0.8);
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.5);
    }

    body.dark-mode .floating-social-only a .tooltiptext::after {
      border-color: transparent rgba(var(--surface-color), 0.8) transparent transparent;
    }

    /* Mobile adjustments for floating social - remains on left */
    @media (max-width: 768px) {
      .floating-social-only {
        position: fixed;
        left: 0;
        top: 0%;
        transform: translateY(50%);
        z-index: 1000;
        background: rgba(var(--heading-color-rgb), 0.1);
        /* Transparent background using RGB var */
        border-radius: 0 15px 15px 0;
        overflow: hidden;
        display: flex;
        flex-direction: row;
        padding: 0px 0px;
        box-shadow: 0px 6px 25px rgba(0, 0, 0, 0.5);
        /* Even stronger shadow */
        align-items: center;
        backdrop-filter: blur(8px);


      }

      .floating-social-only a {
        font-size: 24px;
        padding: 10px;
        width: 45px;
        height: 45px;
      }

      .floating-social-only a:hover {
        transform: translateX(5px) scale(1.1);
        /* Keep original transform */
      }

      .floating-social-only a .tooltiptext {
        left: 100%;
        /* Keep tooltip on right */
        right: unset;
        margin-right: 0;
        margin-left: 10px;
      }

      .floating-social-only a .tooltiptext::after {
        right: 100%;
        /* Keep tooltip arrow on right */
        left: unset;
        border-color: transparent rgba(var(--heading-color-rgb), 0.8) transparent transparent;
      }
    }


    /*--------------------------------------------------------------
    # Preloader
    --------------------------------------------------------------*/
    #preloader {
      position: fixed;
      inset: 0;
      z-index: 999999;
      overflow: hidden;
      background: var(--heading-color);
      transition: all 0.8s ease-out;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    #preloader .spinner-container {
      position: relative;
      width: 80px;
      height: 80px;
    }

    #preloader .spinner-inner {
      position: absolute;
      inset: 0;
      border: 8px solid #ffffff;
      border-color: var(--accent-color) transparent var(--secondary-accent-color) transparent;
      border-radius: 50%;
      width: 80px;
      height: 80px;
      animation: animate-preloader 1.8s cubic-bezier(0.68, -0.55, 0.27, 1.55) infinite;
    }

    #preloader .spinner-text {
      position: absolute;
      inset: 0;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      font-size: 1.2rem;
      font-weight: bold;
      font-family: var(--heading-font);
      animation: pulse 1.5s infinite alternate;
    }

    @keyframes animate-preloader {
      0% {
        transform: rotate(0deg) scale(0.8);
      }

      50% {
        transform: rotate(180deg) scale(1.1);
      }

      100% {
        transform: rotate(360deg) scale(0.8);
      }
    }

    @keyframes pulse {
      0% {
        opacity: 0.7;
        transform: scale(0.9);
      }

      100% {
        opacity: 1;
        transform: scale(1);
      }
    }

    /*--------------------------------------------------------------
    # Scroll Top Button & Theme Toggle Button (NEW Grouping)
    --------------------------------------------------------------*/
    /* Theme Toggle Button (Top Right) */
    .theme-toggle-btn {
      position: fixed;
      top: 15px;
      /* Aligned with hamburger top */
      right: 75px;
      /* Space from hamburger */
      z-index: 1003;
      /* Above mobile nav toggle */
      background-color: var(--accent-color);
      width: 45px;
      height: 45px;
      border-radius: 50%;
      transition: all 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
      box-shadow: 0px 4px 12px hsla(210, 100%, 45%, 0.4);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 15px;
      /* Smaller for better fit in corner */
      color: var(--contrast-color);
      line-height: 0;
      border: none;
      cursor: pointer;
    }

    .theme-toggle-btn:hover {
      background-color: var(--secondary-accent-color);
      color: var(--contrast-color);
      transform: scale(1.1);
      /* Subtle scale on hover */
      box-shadow: 0px 6px 15px hsla(30, 100%, 50%, 0.5);
    }

    /* Scroll Top Button (Bottom Right) */
    #scroll-top {
      position: fixed;
      right: 25px;
      bottom: 25px;
      z-index: 99999;
      background-color: var(--accent-color);
      width: 50px;
      height: 50px;
      border-radius: 50%;
      transition: all 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
      box-shadow: 0px 4px 12px hsla(210, 100%, 45%, 0.4);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 26px;
      color: var(--contrast-color);
      line-height: 0;
      border: none;
      cursor: pointer;
      visibility: hidden;
      opacity: 0;
    }

    #scroll-top.active {
      visibility: visible;
      opacity: 1;
    }

    #scroll-top:hover {
      background-color: var(--secondary-accent-color);
      color: var(--contrast-color);
      transform: translateY(-5px);
      box-shadow: 0px 6px 15px hsla(30, 100%, 50%, 0.5);
    }

    /* Adjust for mobile: Theme toggle moves slightly */
    @media (max-width: 768px) {
      .theme-toggle-btn {
        position: fixed;
        top: 38px;
        right: 75px;
        z-index: 1003;
        background-color: var(--accent-color);
        width: 30px;
        height: 30px;
        border-radius: 50%;
        transition: all 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        box-shadow: 0px 4px 12px hsla(210, 100%, 45%, 0.4);
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 22px;
        color: var(--contrast-color);
        line-height: 0;
        border: none;
        cursor: pointer;
      }

      .theme-toggle-btn:hover {
        background-color: orange;
      }
    }

    #scroll-top {
      width: 45px;
      height: 45px;
      font-size: 22px;
      bottom: 15px;
      right: 15px;
      transform: none;
    }

    #scroll-top:hover {
      transform: scale(1.05);
    }



    /*--------------------------------------------------------------
    # Global Sections
    --------------------------------------------------------------*/
    section,
    .section {
      color: var(--default-color);
      background-color: var(--background-color);
      padding: 80px 0;
      overflow: clip;
      position: relative;
      z-index: 1;
      transition: background-color 0.4s ease, color 0.4s ease;
      /* Smooth theme transition */
    }

    section:nth-child(even) {
      background-color: var(--surface-color) !important;
    }

    section:before {
      content: "";
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-image: radial-gradient(circle at top left, hsla(210, 100%, 45%, 0.05) 0%, transparent 20%),
        radial-gradient(circle at bottom right, hsla(30, 100%, 50%, 0.05) 0%, transparent 20%);
      background-repeat: no-repeat;
      background-size: 40% 40%;
      z-index: -1;
      opacity: 0.5;
    }

    /* Dark mode for section background patterns */
    body.dark-mode section:before {
      background-image: radial-gradient(circle at top left, hsla(210, 100%, 60%, 0.08) 0%, transparent 20%),
        radial-gradient(circle at bottom right, hsla(30, 100%, 65%, 0.08) 0%, transparent 20%);
      opacity: 0.6;
      /* Slightly more visible in dark mode */
    }

    /*--------------------------------------------------------------
    # Global Section Titles (Enhanced)
    --------------------------------------------------------------*/
    .section-title {
      padding-bottom: 70px;
      position: relative;
      text-align: center;
    }

    .section-title h2 {
      font-size: 42px;
      font-weight: 800;
      margin-bottom: 25px;
      padding-bottom: 25px;
      position: relative;
      color: var(--heading-color);
      text-shadow: 2px 2px 5px hsla(210, 20%, 15%, 0.1);
    }

    .section-title h2:after {
      content: "";
      position: absolute;
      display: block;
      width: 80px;
      height: 4px;
      background: linear-gradient(to right, var(--accent-color), var(--secondary-accent-color));
      left: 50%;
      transform: translateX(-50%);
      bottom: 0;
      border-radius: 2px;
    }

    /* Glowing circle effect for section titles */
    .section-title.glowing-circle h2:before {
      content: "";
      position: absolute;
      top: -20px;
      /* Adjust position relative to h2 */
      left: 50%;
      transform: translateX(-50%);
      width: 100px;
      /* Size of the circle */
      height: 100px;
      /* Size of the circle */
      background: radial-gradient(circle, var(--accent-color) 0%, transparent 70%);
      border-radius: 50%;
      opacity: 0.1;
      z-index: -1;
      animation: pulse-glow 3s infinite alternate;
    }

    @keyframes pulse-glow {
      0% {
        transform: translateX(-50%) scale(0.9);
        opacity: 0.1;
      }

      100% {
        transform: translateX(-50%) scale(1.1);
        opacity: 0.25;
      }
    }


    .section-title p {
      margin-bottom: 0;
      color: var(--default-color);
      font-size: 18px;
      line-height: 1.6;
      max-width: 800px;
      margin-left: auto;
      margin-right: auto;
    }

    .section-sub-title {
      font-size: 28px;
      font-weight: 700;
      margin-bottom: 30px;
      color: var(--heading-color);
      text-align: center;
      position: relative;
      padding-bottom: 15px;
    }

    .section-sub-title::after {
      content: '';
      display: block;
      width: 50px;
      height: 3px;
      background: linear-gradient(to right, var(--accent-color), var(--secondary-accent-color));
      margin: 10px auto 0;
      border-radius: 2px;
    }

    /* Dark mode for section sub title */
    body.dark-mode .section-sub-title {
      color: var(--heading-color);
      /* Maintain heading color */
    }

    /*--------------------------------------------------------------
    # Hero Section
    --------------------------------------------------------------*/
    .hero {
      width: 100%;
      min-height: 100vh;
      position: relative;
      padding: 100px 0;
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
      background-color: var(--heading-color);
    }

    .hero img {
      position: absolute;
      inset: 0;
      display: block;
      width: 100%;
      height: 100%;
      object-fit: cover;
      z-index: 1;
      filter: grayscale(80%) brightness(50%);
      transform: scale(1.05);
    }

    .hero:before {
      content: "";
      background: hsla(210, 25%, 15%, 0.8);
      position: absolute;
      inset: 0;
      z-index: 2;
    }

    /* Dark mode for hero overlay */
    body.dark-mode .hero:before {
      background: hsla(210, 25%, 12%, 0.85);
      /* Slightly darker in dark mode */
    }

    .hero .container {
      position: relative;
      z-index: 3;
      text-align: center;
      color: var(--contrast-color);
    }

    .hero h2 {
      margin: 0;
      font-size: 72px;
      font-weight: 800;
      text-shadow: 3px 3px 10px hsla(210, 20%, 15%, 0.4);
      background: linear-gradient(to right, var(--accent-color), var(--secondary-accent-color));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: text-glow 2s infinite alternate;
    }

    @keyframes text-glow {
      0% {
        text-shadow: 0px 0px 10px hsla(210, 100%, 45%, 0.5), 0px 0px 20px hsla(30, 100%, 50%, 0.5);
      }

      100% {
        text-shadow: 0px 0px 15px hsla(210, 100%, 45%, 0.8), 0px 0px 30px hsla(30, 100%, 50%, 0.8);
      }
    }


    .hero p {
      margin: 10px 0 0 0;
      font-size: 30px;
      opacity: 0.9;
      letter-spacing: 2px;
      font-family: var(--nav-font);
    }

    .hero p span {
      letter-spacing: 2px;
      border-bottom: 3px solid var(--secondary-accent-color);
      padding-bottom: 5px;
    }

    @media (max-width: 768px) {
      .hero h2 {
        font-size: 48px;
      }

      .hero p {
        font-size: 24px;
      }
    }

    /*--------------------------------------------------------------
    # About Section (Enhanced)
    --------------------------------------------------------------*/
    .about .content {
      padding-left: 20px;
      /* Add some padding to separate from image */
    }

    .about .content ul {
      list-style: none;
      padding: 0;
    }

    .about .content ul li {
      display: flex;
      /* Use flexbox for icon and text alignment */
      align-items: center;
      /* Vertically center icon and text */
      margin-bottom: 15px;
      /* Add more space between list items */
      font-size: 16px;
      color: var(--default-color);
    }

    .about .content ul li i {
      font-size: 24px;
      /* Larger icons for better visibility */
      color: var(--accent-color);
      /* Use accent color for icons */
      margin-right: 15px;
      /* Space between icon and text */
      min-width: 24px;
      /* Prevent text from jumping if icon width varies */
      text-align: center;
      transition: transform 0.3s ease;
      /* Add hover effect */
    }

    .about .content ul li:hover i {
      transform: scale(1.1);
      /* Slightly enlarge icon on hover */
    }

    .about .content p {
      margin-bottom: 1.5rem;
      /* Consistent spacing for paragraphs */
      line-height: 1.7;
      /* Improve readability */
    }

    /* Adjust the main row in about section for alignment */
    .about .row.gy-4 {
      align-items: center;
      /* Vertically center the image and content columns */
    }

    /* Ensure image responsiveness */
    .about .col-lg-4 img {
      max-width: 100%;
      height: auto;
      border-radius: 12px;
      /* Add some rounded corners to the image */
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
      /* Subtle shadow */
    }

    @media (max-width: 991px) {
      /* On smaller screens, stack columns */
      .about .content {
        padding-left: 0;
        /* Remove left padding when stacked */
        padding-top: 30px;
        /* Add top padding when stacked below image */
      }
    }

    /* Certificates Carousel */
    .certificates-carousel {
      padding: 30px 0;
      overflow: hidden;
      position: relative;
    }

    .certificates-carousel .swiper-slide {
      width: 280px;
      /* Fixed width for each certificate item */
      margin-right: 20px;
      /* Space between items */
    }

    .certificate-item {
      background-color: var(--background-color);
      /* Use background-color var */
      border-radius: 10px;
      padding: 20px;
      text-align: center;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
      transition: all 0.3s ease;
      height: 100%;
      /* Ensure uniform height */
      display: flex;
      flex-direction: column;
      justify-content: center;
      cursor: pointer;
      border: 1px solid rgba(0, 0, 0, 0.05);
      /* Subtle border for separation */
    }

    body.dark-mode .certificate-item {
      background-color: var(--surface-color);
      /* Darker surface in dark mode */
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
      border-color: rgba(255, 255, 255, 0.1);
      /* Lighter border in dark mode */
    }

    .certificate-item:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 15px rgba(0, 0, 0, 0.15);
      background-color: var(--accent-color);
      color: var(--contrast-color);
      border-color: var(--accent-color);
      /* Match border to background on hover */
    }

    body.dark-mode .certificate-item:hover {
      background-color: var(--accent-color);
      color: var(--contrast-color);
      border-color: var(--accent-color);
    }

    .certificate-item .cert-icon {
      font-size: 36px;
      margin-bottom: 10px;
      color: var(--secondary-accent-color);
      transition: color 0.3s ease;
    }

    .certificate-item h4 {
      font-size: 1.2em;
      margin-bottom: 10px;
      color: var(--heading-color);
      transition: color 0.3s ease;
    }

    .certificate-item p {
      font-size: 0.9em;
      color: var(--default-color);
      margin-bottom: 0;
      transition: color 0.3s ease;
    }

    .certificate-item:hover .cert-icon,
    .certificate-item:hover h4,
    .certificate-item:hover p {
      color: var(--contrast-color);
      /* Text color on hover */
    }

    /* Swiper Pagination (dots) */
    .certificates-carousel .swiper-pagination {
      position: static;
      margin-top: 20px;
    }

    .certificates-carousel .swiper-pagination-bullet {
      background: var(--accent-color);
      opacity: 0.6;
    }

    .certificates-carousel .swiper-pagination-bullet-active {
      background: var(--accent-color);
      opacity: 1;
    }

    /* Certificate Details Modal */
    .certificate-details-modal-overlay {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.8);
      display: flex;
      justify-content: center;
      align-items: center;
      z-index: 10000;
      visibility: hidden;
      opacity: 0;
      transition: opacity 0.3s ease-in-out, visibility 0.3s ease-in-out;
    }

    .certificate-details-modal-overlay.active {
      visibility: visible;
      opacity: 1;
    }

    .certificate-details-modal-content {
      background: var(--background-color);
      /* Use background-color var */
      padding: 40px;
      border-radius: 15px;
      box-shadow: 0 8px 30px rgba(0, 0, 0, 0.4);
      max-width: 700px;
      width: 90%;
      max-height: 90%;
      overflow-y: auto;
      position: relative;
      transform: scale(0.9);
      opacity: 0;
      transition: transform 0.3s ease-in-out, opacity 0.3s ease-in-out;
      text-align: center;
      /* Center content in modal */
    }

    .certificate-details-modal-overlay.active .certificate-details-modal-content {
      transform: scale(1);
      opacity: 1;
    }

    body.dark-mode .certificate-details-modal-content {
      background: var(--surface-color);
      /* Darker surface in dark mode */
      box-shadow: 0 8px 30px rgba(0, 0, 0, 0.6);
    }

    .certificate-details-modal-content .close-btn {
      position: absolute;
      top: 15px;
      right: 15px;
      background: none;
      border: none;
      font-size: 30px;
      color: var(--default-color);
      cursor: pointer;
      transition: color 0.3s ease;
    }

    .certificate-details-modal-content .close-btn:hover {
      color: var(--accent-color);
    }

    .certificate-details-modal-content h3 {
      font-size: 2em;
      color: var(--heading-color);
      margin-bottom: 20px;
    }

    .certificate-details-modal-content p {
      font-size: 1.1em;
      line-height: 1.7;
      color: var(--default-color);
      margin-bottom: 20px;
    }

    .certificate-details-modal-content a.btn {
      background-color: var(--accent-color);
      color: var(--contrast-color);
      border-color: var(--accent-color);
      padding: 10px 25px;
      border-radius: 50px;
      font-weight: bold;
      transition: all 0.3s ease;
    }

    .certificate-details-modal-content a.btn:hover {
      background-color: var(--secondary-accent-color);
      border-color: var(--secondary-accent-color);
    }

    /*--------------------------------------------------------------
    # Skills Section (Enhanced)
    ----------------------------------------------------------------*/
    .skills .progress {
      height: 60px;
      display: block;
      background: none;
      border-radius: 0;
      margin-bottom: 30px;
    }

    .skills .progress .skill {
      color: var(--heading-color);
      padding: 0;
      margin: 0 0 8px 0;
      text-transform: uppercase;
      display: flex;
      justify-content: space-between;
      align-items: center;
      /* Align icon and text vertically */
      font-weight: 700;
      font-family: var(--heading-font);
      font-size: 17px;
    }

    .skills .progress .skill i {
      font-size: 22px;
      margin-right: 10px;
      color: var(--accent-color);
      /* Color for skill icons */
      transition: transform 0.3s ease;
    }

    .skills .progress .skill:hover i {
      transform: scale(1.2);
    }

    .skills .progress .skill .val {
      font-style: normal;
      color: var(--accent-color);
    }

    .skills .progress-bar-wrap {
      background: hsla(210, 100%, 45%, 0.1);
      /* Reverted to original light semi-transparent accent blue */
      height: 12px;
      border-radius: 6px;
      overflow: hidden;
      box-shadow: inset 0px 1px 3px hsla(210, 20%, 15%, 0.1);
    }

    /* Dark mode override for skills progress bar background */
    body.dark-mode .skills .progress-bar-wrap {
      background: hsl(210, 10%, 25%);
      /* Reverted to original distinct, slightly lighter dark grey */
      box-shadow: inset 0px 1px 3px hsla(210, 20%, 10%, 0.5);
    }

    .skills .progress-bar {
      width: 1px;
      height: 100%;
      transition: width 1.2s ease-in-out;
      background: linear-gradient(to right, var(--accent-color), var(--secondary-accent-color));
      /* Reverted to original gradient */
      border-radius: 6px;
    }

    /*--------------------------------------------------------------
    # AI Portfolio Section (Redesigned)
    --------------------------------------------------------------*/
    .ai-portfolio-section {
      padding: 80px 0;
      background-color: var(--surface-color);
    }

    .ai-container {
      padding-left: 15px;
      padding-right: 15px;
      margin-left: auto;
      margin-right: auto;
      max-width: 1200px;
    }

    @media (min-width: 768px) {
      .ai-container {
        padding-left: 30px;
        padding-right: 30px;
      }
    }

    .ai-section-title {
      text-align: center;
      padding-bottom: 30px;
    }

    .ai-section-title h2 {
      font-size: 38px;
      font-weight: 700;
      margin-bottom: 10px;
      color: var(--heading-color);
    }

    .ai-section-title p {
      font-size: 18px;
      color: var(--default-color);
    }

    .ai-portfolio-filters {
      list-style: none;
      padding: 0;
      margin: 0 auto 30px auto;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 10px;
      position: relative;
      z-index: 10;
    }

    .ai-portfolio-filters li {
      cursor: pointer;
      padding: 10px 25px;
      background-color: var(--background-color);
      border-radius: 50px;
      font-weight: 600;
      color: var(--default-color);
      transition: all 0.3s ease-in-out;
      border: 1px solid hsla(210, 20%, 15%, 0.1);
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
    }

    .ai-portfolio-filters li.ai-filter-active,
    .ai-portfolio-filters li:hover {
      background-color: var(--accent-color);
      color: var(--contrast-color);
      border-color: var(--accent-color);
      box-shadow: 0 4px 10px hsla(210, 100%, 45%, 0.2);
    }

    /* Dark mode for portfolio filters */
    body.dark-mode .ai-portfolio-filters li {
      background-color: hsl(210, 20%, 25%);
      color: var(--default-color);
      border: 1px solid hsla(210, 20%, 30%, 0.1);
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
    }

    body.dark-mode .ai-portfolio-filters li.ai-filter-active,
    body.dark-mode .ai-portfolio-filters li:hover {
      background-color: var(--accent-color);
      color: var(--contrast-color);
      border-color: var(--accent-color);
      box-shadow: 0 4px 10px hsla(210, 100%, 60%, 0.4);
    }


    .ai-project-card {
      min-height: 350px;
      background-color: var(--background-color);
      /* Use var for background */
      border-radius: 12px;
      box-shadow: 0 6px 15px hsla(210, 20%, 15%, 0.08);
      position: relative;
      overflow: hidden;
      display: flex;
      flex-direction: column;
      justify-content: flex-start;
      /* Align to top */
      align-items: center;
      text-align: center;
      transition: all 0.4s ease-in-out;
      padding: 25px;
      height: 100%;
    }

    .ai-project-card:hover {
      box-shadow: 0 12px 25px hsla(210, 20%, 15%, 0.18);
      transform: translateY(-10px);
    }

    /* Dark mode for project cards */
    body.dark-mode .ai-project-card {
      background-color: var(--surface-color);
      /* Darker cards */
      box-shadow: 0 6px 15px hsla(210, 20%, 15%, 0.3);
      /* Stronger shadows for separation */
    }

    body.dark-mode .ai-project-card:hover {
      box-shadow: 0 12px 25px hsla(210, 20%, 15%, 0.4);
    }


    .ai-project-card .project-icon {
      font-size: 50px;
      color: var(--accent-color);
      margin-bottom: 20px;
      animation: icon-pulse 1.5s infinite alternate;
    }

    @keyframes icon-pulse {
      0% {
        transform: scale(0.95);
        opacity: 0.8;
      }

      100% {
        transform: scale(1);
        opacity: 1;
      }
    }


    .ai-project-title h4 {
      margin: 0;
      color: var(--heading-color);
      font-size: 1.5em;
      /* Adjusted font size */
      line-height: 1.3;
      font-weight: 700;
      margin-bottom: 15px;
    }

    .ai-project-details-overlay {
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background-color: hsla(210, 25%, 15%, 0.95);
      color: #ffffff;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 35px;
      opacity: 0;
      visibility: hidden;
      transition: opacity 0.4s ease-in-out, visibility 0.4s ease-in-out;
    }

    body.dark-mode .ai-project-details-overlay {
      background-color: hsla(210, 25%, 12%, 0.98);
      /* Slightly darker overlay in dark mode */
    }

    .ai-project-card:hover .ai-project-details-overlay {
      opacity: 1;
      visibility: visible;
    }

    .ai-project-details-overlay p {
      margin-bottom: 25px;
      font-size: 1.15em;
      line-height: 1.8;
      max-height: 70%;
      overflow-y: auto;
      font-style: normal;
      /* Ensured no italics */
    }

    .ai-project-links .ai-details-link {
      display: inline-flex;
      align-items: center;
      color: var(--secondary-accent-color);
      background-color: #ffffff;
      padding: 12px 25px;
      border-radius: 30px;
      font-weight: bold;
      font-size: 1em;
      transition: background-color 0.3s ease, color 0.3s ease;
      text-decoration: none;
      /* Ensure no underline */
    }

    body.dark-mode .ai-project-links .ai-details-link {
      background-color: var(--background-color);
      /* Use dark mode background for link */
    }

    .ai-project-links .ai-details-link:hover {
      background-color: var(--surface-color);
      color: hsl(30, 100%, 40%);
    }

    /*--------------------------------------------------------------
    # Resume Section (Enhanced)
    --------------------------------------------------------------*/
    .resume .resume-item {
      padding: 0 0 20px 20px;
      margin-top: -2px;
      border-left: 2px solid var(--accent-color);
      position: relative;
      transition: all 0.3s ease;
    }

    .resume .resume-item:hover {
      border-color: var(--secondary-accent-color);
      background-color: var(--surface-color);
      /* Subtle hover effect */
      border-radius: 0 8px 8px 0;
    }

    /* Dark mode for resume items */
    body.dark-mode .resume .resume-item:hover {
      background-color: hsl(210, 20%, 25%);
    }

    body.dark-mode .resume .resume-item h5 {
      background: hsl(210, 20%, 25%);
      color: var(--default-color);
    }

    .resume .resume-item h4 {
      font-size: 20px;
      font-weight: 700;
      text-transform: uppercase;
      color: var(--heading-color);
      margin-bottom: 10px;
    }

    .resume .resume-item h5 {
      font-size: 16px;
      background: var(--surface-color);
      padding: 5px 15px;
      display: inline-block;
      font-weight: 600;
      margin-bottom: 10px;
      color: var(--default-color);
      border-radius: 5px;
    }

    .resume .resume-item ul {
      padding-left: 20px;
    }

    .resume .resume-item ul li {
      padding-bottom: 10px;
      font-size: 15px;
    }

    .resume .resume-item:last-child {
      padding-bottom: 0;
    }

    .resume .resume-item::before {
      content: "";
      position: absolute;
      width: 16px;
      height: 16px;
      border-radius: 50px;
      left: -9px;
      top: 0;
      background: var(--secondary-accent-color);
      /* Changed to orange */
      border: 2px solid var(--background-color);
      box-shadow: 0 0 8px var(--secondary-accent-color);
      /* Glowing effect */
      transition: all 0.3s ease;
    }

    .resume .resume-item:hover::before {
      background: var(--accent-color);
      /* Blue on hover for contrast */
      box-shadow: 0 0 12px var(--accent-color);
      /* Stronger glow on hover */
    }

    /*--------------------------------------------------------------
    # Services Section (Enhanced - Icons Removed)
    --------------------------------------------------------------*/
    .services .row.gy-4 {
      --bs-gutter-y: 24px;
      /* Consistent vertical gutter */
      --bs-gutter-x: 24px;
      /* Consistent horizontal gutter */
    }

    .services .service-item {
      position: relative;
      cursor: pointer;
      background-color: var(--background-color);
      /* Use var for background */
      border-radius: 12px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08);
      transition: all 0.3s ease-in-out;
      padding: 30px;
      /* Increased padding inside the card */
      height: 100%;
      /* Ensure uniform height for grid alignment */
      display: flex;
      flex-direction: column;
      /* Changed to column layout */
      align-items: center;
      /* Center items horizontally */
      text-align: center;
      /* Center text */
    }

    .services .service-item:hover {
      transform: translateY(-8px);
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
    }

    /* Dark mode for service items */
    body.dark-mode .services .service-item {
      background-color: var(--surface-color);
      /* Darker cards */
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
      /* Stronger shadows for separation */
    }


    /* Icon styles removed */
    .services .service-item .icon {
      display: none;
      /* Hide the icon */
    }


    .services .service-item div {
      /* This targets the div containing h4 and p */
      text-align: center;
      /* Ensure text is centered within the card */
      flex-grow: 1;
      /* Allow text content to take available space */
    }

    .services .service-item h4.title {
      font-size: 22px;
      /* Slightly larger title */
      margin-bottom: 15px;
      /* Increased margin-bottom for better separation */
      color: var(--heading-color);
      line-height: 1.3;
      margin-top: 0;
      /* Ensure no unwanted margin-top */
    }

    .services .service-item p.description {
      font-size: 15px;
      line-height: 1.7;
      color: var(--default-color);
      margin-bottom: 0;
      margin-top: 0;
      /* Ensure no unwanted margin-top */
    }


    /* Service Details Modal Overlay */
    .service-details-modal-overlay {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.8);
      /* Dark semi-transparent background */
      display: flex;
      justify-content: center;
      align-items: center;
      z-index: 10000;
      visibility: hidden;
      opacity: 0;
      transition: opacity 0.3s ease-in-out, visibility 0.3s ease-in-out;
    }

    .service-details-modal-overlay.active {
      visibility: visible;
      opacity: 1;
    }

    .service-details-modal-content {
      background: var(--background-color);
      /* Use background-color var */
      padding: 40px;
      border-radius: 15px;
      box-shadow: 0 8px 30px rgba(0, 0, 0, 0.4);
      max-width: 800px;
      width: 90%;
      max-height: 90%;
      overflow-y: auto;
      position: relative;
      transform: scale(0.9);
      opacity: 0;
      transition: transform 0.3s ease-in-out, opacity 0.3s ease-in-out;
    }

    .service-details-modal-overlay.active .service-details-modal-content {
      transform: scale(1);
      opacity: 1;
    }

    /* Dark mode for service details modal */
    body.dark-mode .service-details-modal-content {
      background: var(--surface-color);
      /* Darker surface */
      box-shadow: 0 8px 30px rgba(0, 0, 0, 0.6);
    }

    body.dark-mode .service-details-modal-content h3 {
      color: var(--heading-color);
    }

    body.dark-mode .service-details-modal-content p {
      color: var(--default-color);
    }

    .service-details-modal-content .close-btn {
      position: absolute;
      top: 20px;
      right: 20px;
      background: none;
      border: none;
      font-size: 30px;
      color: var(--default-color);
      cursor: pointer;
      transition: color 0.3s ease;
    }

    .service-details-modal-content .close-btn:hover {
      color: var(--accent-color);
    }

    .service-details-modal-content h3 {
      font-size: 32px;
      color: var(--heading-color);
      margin-bottom: 20px;
      text-align: center;
    }

    .service-details-modal-content p {
      font-size: 16px;
      line-height: 1.8;
      color: var(--default-color);
      text-align: left;
    }

    /* Adjust service item link to be clickable anywhere within the card */
    .services .service-item .stretched-link {
      position: absolute;
      width: 100%;
      height: 100%;
      top: 0;
      left: 0;
      z-index: 1;
      /* Ensure it's above other elements but below overlay content */
      cursor: pointer;
    }

    .services .service-item {
      position: relative;
      cursor: pointer;
      /* Indicate clickability */
    }

    /*--------------------------------------------------------------
    # Testimonials Section (Polished - No Images)
    --------------------------------------------------------------*/
    .testimonials .testimonial-item {
      padding: 30px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08);
      background: var(--background-color);
      /* Use background-color var */
      border-radius: 12px;
      height: auto;
      /* Allow height to adjust based on content */
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      margin-top: 30px;
      /* Space from the top of its container */
      transition: all 0.3s ease;
    }

    .testimonials .testimonial-item:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
    }

    /* Dark mode for testimonials */
    body.dark-mode .testimonials .testimonial-item {
      background: var(--surface-color);
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
    }

    body.dark-mode .testimonials .testimonial-item h3 {
      color: var(--heading-color);
    }

    body.dark-mode .testimonials .testimonial-item h4 {
      color: var(--accent-color);
    }


    .testimonials .testimonial-item p {
      font-style: italic;
      margin: 0 0 15px 0;
      font-size: 16px;
      line-height: 1.8;
      position: relative;
      padding: 10px 0;
    }

    .testimonials .testimonial-item .quote-icon-left,
    .testimonials .testimonial-item .quote-icon-right {
      color: var(--secondary-accent-color);
      /* Orange color for quotes */
      font-size: 26px;
      line-height: 1;
    }

    .testimonials .testimonial-item .quote-icon-left {
      position: absolute;
      left: -10px;
      top: -5px;
    }

    .testimonials .testimonial-item .quote-icon-right {
      position: absolute;
      right: -10px;
      bottom: -5px;
    }

    .testimonials .testimonial-img {
      display: none;
      /* Hide images as requested */
    }

    .testimonials .testimonial-item h3 {
      font-size: 20px;
      font-weight: 700;
      margin: 10px 0 5px 0;
      color: var(--heading-color);
      text-transform: capitalize;
      /* More natural capitalization */
    }

    .testimonials .testimonial-item h4 {
      font-size: 14px;
      color: var(--accent-color);
      /* Accent color for title */
      margin: 0;
      text-transform: uppercase;
    }

    .testimonials .swiper-pagination {
      margin-top: 20px;
      position: relative;
      bottom: auto;
      left: auto;
    }

    .testimonials .swiper-pagination .swiper-pagination-bullet {
      width: 12px;
      height: 12px;
      background-color: hsla(210, 100%, 45%, 0.3);
      /* Lighter accent color */
      opacity: 1;
      border-radius: 50%;
      margin: 0 6px;
      transition: all 0.3s ease;
    }

    .testimonials .swiper-pagination .swiper-pagination-bullet-active {
      background-color: var(--accent-color);
      /* Vibrant accent color when active */
      transform: scale(1.2);
    }

    /* Footer styling */
    footer {
      padding-top: 60px;
      /* Increased top padding to make its start more visible */
      padding-bottom: 20px;
      background-color: var(--surface-color);
      /* Use a distinct background color if needed */
      color: var(--default-color);
      text-align: center;
      font-size: 14px;
      margin-top: 0;
      /* Ensure no extra margin pushes it away */
    }

    /* Dark mode for footer */
    body.dark-mode footer {
      background-color: hsl(210, 20%, 15%);
      color: hsl(210, 10%, 80%);
    }

    /*--------------------------------------------------------------
    # Contact Section Enhancements
    --------------------------------------------------------------*/
    .contact .info-wrap {
      background-color: var(--background-color);
      /* Use var for background */
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
      height: 100%;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }

    /* Dark mode for contact info-wrap */
    body.dark-mode .contact .info-wrap {
      background-color: var(--surface-color);
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
    }

    .contact .info-item {
      margin-bottom: 25px;
      background-color: var(--surface-color);
      padding: 15px 20px;
      border-radius: 8px;
      transition: all 0.3s ease;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
    }

    .contact .info-item:hover {
      transform: translateY(-3px);
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    }

    /* Dark mode for contact info-item */
    body.dark-mode .contact .info-item {
      background-color: hsl(210, 20%, 25%);
      /* Even darker for info items */
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.2);
    }

    .contact .info-item i {
      font-size: 30px;
      color: var(--accent-color);
      line-height: 1;
      margin-right: 20px;
    }

    .contact .info-item h3 {
      font-size: 20px;
      font-weight: 700;
      margin-bottom: 5px;
      color: var(--heading-color);
    }

    .contact .info-item p {
      font-size: 15px;
      margin-bottom: 0;
      color: var(--default-color);
    }

    .contact iframe {
      border-radius: 12px;
      margin-top: 25px;
      height: 270px;
      /* Ensure consistent height */
      width: 100%;
      /* Ensure responsiveness */
      filter: grayscale(20%);
      /* Subtle grayscale for theme consistency */
      transition: filter 0.3s ease;
    }

    body.dark-mode .contact iframe {
      filter: grayscale(50%) brightness(0.8);
      /* More muted in dark mode */
    }

    .contact iframe:hover {
      filter: grayscale(0%);
      /* Full color on hover */
    }

    .contact .php-email-form {
      background-color: var(--background-color);
      /* Use var for background */
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
      height: 100%;
      /* Match height with info-wrap */
    }

    /* Dark mode for contact form */
    body.dark-mode .contact .php-email-form {
      background-color: var(--surface-color);
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
    }

    .contact .php-email-form .form-control {
      border-radius: 8px;
      border: 1px solid var(--surface-color);
      /* Initial border */
      padding: 12px 15px;
      box-shadow: none;
      transition: all 0.3s ease;
      background-color: var(--background-color);
      /* Use background-color var for input */
    }

    .contact .php-email-form .form-control:focus {
      border-color: var(--accent-color);
      box-shadow: 0 0 0 0.25rem hsla(210, 100%, 45%, 0.25);
    }

    /* Dark mode for form controls */
    body.dark-mode .contact .php-email-form .form-control {
      background-color: hsl(210, 20%, 20%);
      /* Darker input fields */
      color: var(--default-color);
      border-color: hsl(210, 20%, 35%);
      /* Clearer border in dark mode */
    }

    body.dark-mode .contact .php-email-form .form-control::placeholder {
      color: hsl(210, 10%, 60%);
    }

    body.dark-mode .contact .php-email-form .form-control:focus {
      border-color: var(--accent-color);
      box-shadow: 0 0 0 0.25rem hsla(210, 100%, 60%, 0.25);
    }

    .contact .php-email-form label {
      font-weight: 600;
      font-size: 15px;
      color: var(--heading-color);
      margin-bottom: 8px;
      /* Added margin */
    }

    .contact .php-email-form button[type="submit"] {
      background: linear-gradient(to right, var(--accent-color), var(--secondary-accent-color));
      border: 0;
      padding: 14px 40px;
      color: #fff;
      transition: 0.4s;
      border-radius: 50px;
      box-shadow: 0 4px 15px hsla(210, 100%, 45%, 0.4);
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    .contact .php-email-form button[type="submit"]:hover {
      transform: translateY(-3px);
      box-shadow: 0 8px 20px hsla(210, 100%, 45%, 0.6);
    }

    /* Dark mode for php-email-form loading */
    body.dark-mode .php-email-form .loading {
      background: var(--surface-color);
    }
  </style>
</head>

<body class="index-page">

  <!-- Preloader -->
  <div id="preloader">
    <div class="spinner-container">
      <div class="spinner-inner"></div>
      <div class="spinner-text">Loading...</div>
    </div>
  </div>

  <!-- Header (for desktop navigation and mobile toggle) -->
  <header id="header" class="header d-flex align-items-center">
    <!-- Wrap logo in a div to easily hide/show it -->
    <div class="logo-container">
      <a href="index.html" class="logo d-flex align-items-center me-auto me-xl-0">

      </a>
    </div>


    <!-- Main Navigation (Desktop Only) -->
    <nav id="main-nav" class="main-nav">
      <ul>
        <li><a href="#hero" class="scrollto active">Home</a></li>
        <li><a href="#skills" class="scrollto">Skills</a></li>
        <li><a href="#ai-portfolio" class="scrollto">Portfolio</a></li>
        <li><a href="#resume" class="scrollto">Resume</a></li>
        <li><a href="#services" class="scrollto">Services</a></li>
        <li><a href="#contact" class="scrollto">Contact</a></li>
      </ul>
    </nav>


    <!-- Mobile Navigation Toggle (Hamburger) -->
    <button class="mobile-nav-toggle d-xl-none bi bi-list"></button>

    <!-- Mobile Navigation Menu (Hidden by default) -->
    <nav class="mobile-nav d-xl-none" style="margin-top: 200px;">
      <ul>
        <li><a href="#hero" class="scrollto active">Home</a></li>
        <li><a href="#skills" class="scrollto">Skills</a></li>
        <li><a href="#ai-portfolio" class="scrollto">Portfolio</a></li>
        <li><a href="#resume" class="scrollto">Resume</a></li>
        <li><a href="#services" class="scrollto">Services</a></li>
        <li><a href="#contact" class="scrollto">Contact</a></li>
      </ul>
    </nav>

  </header>

  <!-- Floating Social Only (Left) -->
  <div class="floating-social-only">
    <a href="https://linkedin.com/in/clayton-gwava" target="_blank" title="LinkedIn">
      <i class="fab fa-linkedin-in"></i>
      <span class="tooltiptext">LinkedIn</span>
    </a>
    <a href="https://github.com/ClaytonGwava" target="_blank" title="GitHub">
      <i class="fab fa-github"></i>
      <span class="tooltiptext">GitHub</span>
    </a>
    <a href="https://www.instagram.com/claytongwava?igsh=MXVpZzBnZWllbTRicw%3D%3D&utm_source=qr" target="_blank" title="Instagram">
      <i class="fab fa-instagram"></i>
      <span class="tooltiptext">Instagram</span>
    </a>
    <a href="tel:641-819-1309" title="call">
      <i class="fas fa-phone"></i>
      <span class="tooltiptext">Call</span>
    </a>
    <a href="mailto:csgwava@gmail.com" title="Email">
      <i class="fas fa-envelope"></i>
      <span class="tooltiptext">Email</span>
    </a>
    <a href="https://twitter.com/ClaytonGwava" target="_blank" aria-label="Twitter">
      <i class="fab fa-twitter"></i>
      <span class="tooltiptext">Twitter</span>
    </a>

  </div>

  <!-- Theme Toggle Button (Top Right) -->
  <button id="themeToggle" class="theme-toggle-btn" title="Toggle Dark/Light Mode">
    <i class="bi bi-sun"></i>
    <!-- Sun icon for light mode -->
    <i class="bi bi-moon" style="display:none;"></i>
    <!-- Moon icon for dark mode, hidden initially -->
  </button>

  <!-- Scroll Top Button (Bottom Right) -->
  <a href="#" id="scroll-top" class="scroll-top d-flex align-items-center justify-content-center"><i class="bi bi-arrow-up-short"></i></a>


  <main class="main">

    <!-- Hero Section -->
    <section id="hero" class="hero section dark-background">
      <img src="assets/img/ai_background.jpg" alt="Futuristic AI Network Background" data-aos="fade-in" loading="lazy">

      <div class="container" data-aos="fade-up" data-aos-delay="100">
        <h2>Clayton Gwava</h2>
        <p>I'm a <span class="typed" data-typed-items="GenAI Engineer, LLM-Powered Systems Architect, Machine Learning Engineer, Data Scientist, AI Ethicist">GenAI Engineer</span><span class="typed-cursor typed-cursor--blink" aria-hidden="true"></span></p>
      </div>
    </section><!-- /Hero Section -->

    <!-- About Section -->
    <section id="about" class="about section">
      <div class="container section-title glowing-circle" data-aos="fade-up">
        <h2>About Me</h2>
        <p>AI Engineer with deep expertise in Generative AI and LLMs. I build intelligent systems that solve real-world problems and drive innovation.</p>
      </div>

      <div class="container" data-aos="fade-up" data-aos-delay="100">
        <div class="row gy-4 justify-content-center">
          <div class="col-lg-4">
            <img src="https://placehold.co/400x500/212529/FFFFFF/png?text=Clayton+Gwava+Portrait" class="img-fluid" alt="Clayton Gwava Portrait" loading="lazy">
          </div>
          <div class="col-lg-8 content">
            <h2>GenAI Engineer | LLM Systems | Scalable Chatbots</h2>
            <p class="py-3">
              My expertise spans LLM-powered systems, fine-tuning, RAG, and building scalable chatbots. I transform complex data into actionable insights and build robust AI models.
            </p>
            <div class="row">
              <div class="col-lg-6">
                <ul>
                  <li><i class="bi bi-cpu"></i> <strong>Specialization:</strong> <span>GenAI Engineer</span></li>
                  <li><i class="bi bi-phone"></i> <strong>Phone:</strong> <a href="tel:641-819-1309"><span>641-819-1309</span></a></li>
                  <li><i class="bi bi-geo-alt"></i> <strong>Location:</strong> <span>Fairfield, Iowa, 52556</span></li>
                </ul>
              </div>
              <div class="col-lg-6">
                <ul>
                  <li><i class="bi bi-calendar-event"></i> <strong>Experience:</strong> <span>8+ Years</span></li>
                  <li style="margin-right: 2px;"><i class="bi bi-journal-check"></i> <strong>Degree:</strong> <span>M.Sc. CompSci</span></li>
                  <li><i class="bi bi-envelope"></i> <strong>Email:</strong> <a href="mailto:csgwava@gmail.com"><span>csgwava@gmail.com</span></a></li>
                  <li><i class="bi bi-briefcase"></i> <strong>Availability:</strong> <span>Open to Projects</span></li>
                </ul>
              </div>
            </div>
            <p class="py-3">
              I develop scalable chatbot applications, customize open-source LLMs, and deploy AI solutions using LangChain, Hugging Face, and vector databases. Strong in backend (Java, Python, Docker, FastAPI), I architect powerful, scalable, and business-aligned AI systems. My mission: use Generative AI responsibly for impactful tools.
            </p>
          </div>
        </div>

        <!-- Certificates & Courses Carousel (NEW) -->
        <div class="col-lg-12 mt-5">
          <h3 class="section-sub-title">Certificates & Courses</h3>
          <p style="text-align: center;">Review My Completed Certifications and Courses</p>


          <div class="certificates-carousel swiper">

            <div class="swiper-wrapper align-items-center">
              <!-- Certificate Item 1 -->
              <div class="swiper-slide">
                <div class="certificate-item" data-certificate-id="cert1">
                  <i class="fab fa-google cert-icon"></i>
                  <h4>Google Professional ML Engineer</h4>
                  <p>Google Cloud</p>
                </div>
              </div>
              <!-- Certificate Item 2 -->
              <div class="swiper-slide">
                <div class="certificate-item" data-certificate-id="cert2">
                  <i class="bi bi-diagram-3-fill cert-icon"></i>
                  <h4>TOGAF 9 Practitioner</h4>
                  <p>The Open Group</p>
                </div>
              </div>
              <!-- Certificate Item 3 -->
              <div class="swiper-slide">
                <div class="certificate-item" data-certificate-id="cert3">
                  <i class="bi bi-journal-richtext cert-icon"></i>
                  <h4>PRINCE2 Agile Practitioner</h4>
                  <p>AXELOS</p>
                </div>
              </div>
              <!-- Certificate Item 4 -->
              <div class="swiper-slide">
                <div class="certificate-item" data-certificate-id="cert4">
                  <i class="bi bi-bar-chart-fill cert-icon"></i>
                  <h4>Applied Data Science 1</h4>
                  <p>Provider Name</p>
                </div>
              </div>
              <!-- Certificate Item 5 -->
              <div class="swiper-slide">
                <div class="certificate-item" data-certificate-id="cert5">
                  <i class="bi bi-mortarboard-fill cert-icon"></i>
                  <h4>Machine Learning Specialization</h4>
                  <p>DeepLearning.AI | Coursera</p>
                </div>
              </div>
              <!-- Certificate Item 6 -->
              <div class="swiper-slide">
                <div class="certificate-item" data-certificate-id="cert6">
                  <i class="fas fa-robot cert-icon"></i>
                  <h4>Generative AI with Transformers</h4>
                  <p>Hugging Face | Coursera</p>
                </div>
              </div>
              <!-- Certificate Item 7 -->
              <div class="swiper-slide">
                <div class="certificate-item" data-certificate-id="cert7">
                  <i class="bi bi-stack cert-icon"></i>
                  <h4>Deep Learning Specialization</h4>
                  <p>DeepLearning.AI | Coursera</p>
                </div>
              </div>
              <!-- Certificate Item 8 -->
              <div class="swiper-slide">
                <div class="certificate-item" data-certificate-id="cert8">
                  <i class="bi bi-arrow-repeat cert-icon"></i>
                  <h4>Reinforcement Learning</h4>
                  <p>University of Alberta | Coursera</p>
                </div>
              </div>
              <!-- Certificate Item 9 -->
              <div class="swiper-slide">
                <div class="certificate-item" data-certificate-id="cert9">
                  <i class="bi bi-shield-lock-fill cert-icon"></i>
                  <h4>Cisco Cybersecurity</h4>
                  <p>Cisco Networking Academy</p>
                </div>
              </div>
              <!-- Certificate Item 10 -->
              <div class="swiper-slide">
                <div class="certificate-item" data-certificate-id="cert10">
                  <i class="fab fa-linux cert-icon"></i>
                  <h4>Linux Essentials</h4>
                  <p>Cisco Networking Academy</p>
                </div>
              </div>
              <!-- Certificate Item 11 -->
              <div class="swiper-slide">
                <div class="certificate-item" data-certificate-id="cert11">
                  <i class="bi bi-wifi cert-icon"></i>
                  <h4>Mobility Fundamental</h4>
                  <p>Cisco Networking Academy</p>
                </div>
              </div>
              <!-- Certificate Item 12 -->
              <div class="swiper-slide">
                <div class="certificate-item" data-certificate-id="cert12">
                  <i class="bi bi-calculator-fill cert-icon"></i>
                  <h4>Scientific Computing & Python for Data Science</h4>
                  <p>WorldQuant University</p>
                </div>
              </div>
              <!-- Add more certificate items as needed -->
            </div>
            <div class="swiper-pagination"></div>
          </div>
        </div>
      </div>
    </section><!-- /About Section -->

    <!-- Skills Section -->
    <section id="skills" class="skills section">
      <div class="container section-title glowing-circle" data-aos="fade-up">
        <h2>Technical Skills</h2>
        <p>Broad expertise in AI, software engineering, and data science.</p>
      </div>

      <div class="container" data-aos="fade-up" data-aos-delay="100">
        <div class="row skills-content skills-animation">
          <div class="col-lg-6">
            <div class="progress">
              <span class="skill"> <i class="fab fa-python"></i> <span>Python</span> <i class="val">100%</i></span>
              <div class="progress-bar-wrap">
                <div class="progress-bar" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>
            <div class="progress">
              <span class="skill"> <i class="fab fa-java"></i> <span>Java & Spring Boot</span> <i class="val">100%</i></span>
              <div class="progress-bar-wrap">
                <div class="progress-bar" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>
            <div class="progress">
              <span class="skill"> <i class="bi bi-robot"></i> <span>LLMs & NLP (Prompt Eng., Fine-tuning, Embeddings, LangChain)</span> <i class="val">90%</i></span>
              <div class="progress-bar-wrap">
                <div class="progress-bar" role="progressbar" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>
            <div class="progress">
              <span class="skill"> <i class="bi bi-bar-chart-fill"></i> <span>Data Science, Cleaning & Feature Engineering</span> <i class="val">88%</i></span>
              <div class="progress-bar-wrap">
                <div class="progress-bar" role="progressbar" aria-valuenow="88" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>
          </div>
          <div class="col-lg-6">
            <div class="progress">
              <span class="skill"> <i class="bi bi-cpu"></i> <span>Machine Learning Algorithms (Scikit-learn, TensorFlow, PyTorch)</span> <i class="val">95%</i></span>
              <div class="progress-bar-wrap">
                <div class="progress-bar" role="progressbar" aria-valuenow="95" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>
            <div class="progress">
              <span class="skill"> <i class="bi bi-stack"></i> <span>Deep Learning (TensorFlow, PyTorch, Hugging Face Transformers)</span> <i class="val">92%</i></span>
              <div class="progress-bar-wrap">
                <div class="progress-bar" role="progressbar" aria-valuenow="92" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>
            <div class="progress">
              <span class="skill"> <i class="bi bi-cloud-fill"></i> <span>Cloud, DevOps & MLOps Tools (AWS S3/RDS/DynamoDB/SageMaker/Lambda, Jenkins, FastAPI, Streamlit, Git)</span> <i class="val">85%</i></span>
              <div class="progress-bar-wrap">
                <div class="progress-bar" role="progressbar" aria-valuenow="85" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section><!-- /Skills Section -->

    <!-- AI Portfolio Section (Redesigned) -->
    <section id="ai-portfolio" class="ai-portfolio-section ai-light-background">
      <div class="container section-title glowing-circle" data-aos="fade-up">
        <h2 style="color: var(--heading-color); font-weight: bold;">AI Portfolio</h2>
        <p style="color: var(--default-color);">My impactful AI projects: LLMs, deep learning, data analytics.</p>
      </div>
      <div class="ai-container">
        <div class="ai-isotope-layout" data-default-filter="*" data-layout="masonry" data-sort="original-order">
          <ul class="ai-portfolio-filters ai-isotope-filters" data-aos="fade-up" data-aos-delay="100">
            <li data-filter="*" class="ai-filter-active">All</li>
            <li data-filter=".ai-filter-llm">LLM Solutions</li>
            <li data-filter=".ai-filter-ml">Machine Learning</li>
            <li data-filter=".ai-filter-dl">Deep Learning</li>
            <li data-filter=".ai-filter-data">Data Analytics</li>
          </ul>
          <div class="row gy-4 ai-isotope-container" data-aos="fade-up" data-aos-delay="200">
            <div class="col-lg-4 col-md-6 ai-portfolio-item ai-isotope-item ai-filter-llm">
              <div class="ai-project-card ai-h-100">
                <i class="bi bi-chat-dots-fill project-icon"></i>
                <div class="ai-project-title">
                  <h4>Scalable LLM Chatbot</h4>
                </div>
                <div class="ai-project-details-overlay">
                  <p>Developed a multilingual chatbot using fine-tuned LLMs and RAG, reducing contact center traffic.</p>
                  <div class="ai-project-links">
                    <a href="#" title="More Details" class="ai-details-link">Details <i class="bi bi-arrow-right"></i></a>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-lg-4 col-md-6 ai-portfolio-item ai-isotope-item ai-filter-ml">
              <div class="ai-project-card ai-h-100">
                <i class="bi bi-person-x-fill project-icon"></i>
                <div class="ai-project-title">
                  <h4>Customer Churn Prediction</h4>
                </div>
                <div class="ai-project-details-overlay">
                  <p>Deployed a churn prediction model that improved customer retention by 15% through targeted campaigns.</p>
                  <div class="ai-project-links">
                    <a href="#" title="More Details" class="ai-details-link">Details <i class="bi bi-arrow-right"></i></a>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-lg-4 col-md-6 ai-portfolio-item ai-isotope-item ai-filter-dl">
              <div class="ai-project-card ai-h-100">
                <i class="bi bi-graph-up-arrow project-icon"></i>
                <div class="ai-project-title">
                  <h4>Network Traffic Forecasting</h4>
                </div>
                <div class="ai-project-details-overlay">
                  <p>LSTM models for precise network traffic forecasting, improving uptime by 12%.</p>
                  <div class="ai-project-links">
                    <a href="#" title="More Details" class="ai-details-link">Details <i class="bi bi-arrow-right"></i></a>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-lg-4 col-md-6 ai-portfolio-item ai-isotope-item ai-filter-data">
              <div class="ai-project-card ai-h-100">
                <i class="bi bi-people-fill project-icon"></i>
                <div class="ai-project-title">
                  <h4>Customer Segmentation</h4>
                </div>
                <div class="ai-project-details-overlay">
                  <p>Unsupervised techniques for personalized marketing strategies.</p>
                  <div class="ai-project-links">
                    <a href="#" title="More Details" class="ai-details-link">Details <i class="bi bi-arrow-right"></i></a>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-lg-4 col-md-6 ai-portfolio-item ai-isotope-item ai-filter-ml">
              <div class="ai-project-card ai-h-100">
                <i class="bi bi-shield-slash-fill project-icon"></i>
                <div class="ai-project-title">
                  <h4>Fraud Anomaly Detection</h4>
                </div>
                <div class="ai-project-details-overlay">
                  <p>Real-time anomaly detection for fraud prevention, saving significant losses.</p>
                  <div class="ai-project-links">
                    <a href="#" title="More Details" class="ai-details-link">Details <i class="bi bi-arrow-right"></i></a>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-lg-4 col-md-6 ai-portfolio-item ai-isotope-item ai-filter-llm">
              <div class="ai-project-card ai-h-100">
                <i class="bi bi-tools project-icon"></i>
                <div class="ai-project-title">
                  <h4>Industry LLM Fine-Tuning</h4>
                </div>
                <div class="ai-project-details-overlay">
                  <p>Customized LLMs for specific industry applications, enhancing domain understanding.</p>
                  <div class="ai-project-links">
                    <a href="#" title="More Details" class="ai-details-link">Details <i class="bi bi-arrow-right"></i></a>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-lg-4 col-md-6 ai-portfolio-item ai-isotope-item ai-filter-ml">
              <div class="ai-project-card ai-h-100">
                <i class="bi bi-award-fill project-icon"></i>
                <div class="ai-project-title">
                  <h4>Hyper-Personalization System</h4>
                </div>
                <div class="ai-project-details-overlay">
                  <p>Advanced recommendation systems boosting engagement and revenue for MNO customers.</p>
                  <div class="ai-project-links">
                    <a href="#" title="More Details" class="ai-details-link">Details <i class="bi bi-arrow-right"></i></a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section><!-- /AI Portfolio Section -->

    <!-- Resume Section -->
    <section id="resume" class="resume section">
      <div class="container section-title glowing-circle" data-aos="fade-up">
        <h2>Resume</h2>
        <p>My professional journey in AI and technology.</p>
      </div>

      <div class="container">
        <div class="row">
          <div class="col-lg-6" data-aos="fade-up" data-aos-delay="100">
            <h3 class="resume-title">Summary</h3>
            <div class="resume-item pb-0">
              <h4>Clayton Gwava</h4>
              <p>AI Engineer specializing in LLM systems, fine-tuning, and RAG. I architect powerful, scalable, and business-aligned AI solutions.</p>
              <ul>
                <li>Fairfield, Iowa, 52556</li>
                <li><a href="tel:641-819-1309">641-819-1309</a></li>
                <li><a href="mailto:csgwava@gmail.com">csgwava@gmail.com</a></li>
              </ul>
            </div>

            <h3 class="resume-title">Education</h3>
            <div class="resume-item">
              <h4>M.Sc. Computer Science</h4>
              <h5>Oct 2024 - Jun 2027 (Expected)</h5>
              <p>Maharishi International University, USA</p>
              <ul>
                <li>Advanced software engineering, data structures, algorithms.</li>
              </ul>
            </div>
            <div class="resume-item">
              <h4>B.Sc. Electrical Engineering</h4>
              <h5>2013 - 2017</h5>
              <p>University of Zimbabwe</p>
              <ul>
                <li>Problem-solving and analytical thinking.</li>
              </ul>
            </div>
            <div class="resume-item">
              <h4>Cert. Data Analytics</h4>
              <h5>2019 - 2020</h5>
              <p>Hash Analytic, India</p>
              <ul>
                <li>Data analysis, visualization, ML application.</li>
              </ul>
            </div>
            <div class="resume-item">
              <h4>Project Management</h4>
              <h5>2019 - 2020</h5>
              <p>University of Zimbabwe</p>
              <ul>
                <li>Project planning, execution, monitoring.</li>
              </ul>
            </div>
            <div class="resume-item">
              <h4>IT Admin & Mgmt</h4>
              <h5>2017 - 2018</h5>
              <p>Cisco Networking Academy</p>
              <ul>
                <li>Network admin, IT infrastructure, system management.</li>
              </ul>
            </div>
            <div class="resume-item">
              <h4>Scientific Computing & Python for Data Science</h4>
              <h5>2020</h5>
              <p>WorldQuant University</p>
              <ul>
                <li>Python for data manipulation, analysis, visualization.</li>
              </ul>
            </div>

            <h3 class="resume-title">Certifications</h3>
            <div class="resume-item">
              <ul>
                <li>Google Professional ML Engineer</li>
                <li>TOGAF 9 Practitioner</li>
                <li>PRINCE2 Agile Practitioner</li>
                <li>Applied Data Science 1</li>
                <li>Machine Learning Specialization</li>
                <li>Generative AI with Transformers</li>
                <li>Advanced NLP with TensorFlow</li>
                <li>Deep Learning Specialization</li>
                <li>Reinforcement Learning</li>
                <li>Cisco Cybersecurity</li>
                <li>Cisco Networking Academy: Linux Essentials</li>
                <li>Cisco Networking Academy: Mobility Fundamental</li>
                <li>Scientific Computing & Python for Data Science</li>
              </ul>
            </div>
          </div>

          <div class="col-lg-6" data-aos="fade-up" data-aos-delay="200">
            <h3 class="resume-title">Professional Experience</h3>
            <div class="resume-item">
              <h4>AI Engineer</h4>
              <h5>May 2021 - Nov 2024</h5>
              <p>Econet Wireless Zimbabwe</p>
              <ul>
                <li>Designed & deployed AI for telecom operations; improved churn prediction (15% retention).</li>
                <li>Developed customer segmentation for personalized marketing.</li>
                <li>Implemented network traffic forecasting (LSTM); 12% uptime improvement.</li>
                <li>Led fraud anomaly detection (SIM swap, usage patterns); prevented significant losses.</li>
                <li>Supported NLP chatbot (WhatsApp, African languages); reduced support workload by 30%.</li>
                <li>Experienced with foundational models; developed hyper-personalization systems for MNOs.</li>
              </ul>
            </div>
            <div class="resume-item">
              <h4>Billing/VAS Systems Engineer</h4>
              <h5>Jun 2019 - Apr 2021</h5>
              <p>Econet Wireless Zimbabwe</p>
              <ul>
                <li>Aligned tech with business strategy; supported revenue/customer growth.</li>
                <li>Led planning & implementation of scalable telecom systems.</li>
                <li>Designed system topologies & capacity plans.</li>
                <li>Spearheaded disaster recovery for IN/Billing/VAS systems.</li>
              </ul>
            </div>
            <div class="resume-item">
              <h4>Intern</h4>
              <h5>Feb 2020 - Jun 2020</h5>
              <p>Harsh Analytic, India</p>
              <ul>
                <li>Performed data analytics (Python, Tableau, Google Analytics).</li>
                <li>Solved real-time problems with ML/AI.</li>
              </ul>
            </div>
            <div class="resume-item">
              <h4>Graduate Systems Engineer</h4>
              <h5>Jun 2018 - May 2019</h5>
              <p>Econet Wireless Zimbabwe</p>
              <ul>
                <li>Supported enterprise system design & maintenance.</li>
                <li>Automated deployment with Bash/Python.</li>
                <li>Monitored networks, contributed to security updates.</li>
              </ul>
            </div>
            <div class="resume-item">
              <h4>Automation Engineer</h4>
              <h5>Jun 2017 - Apr 2018</h5>
              <p>ERG Africa, DRC</p>
              <ul>
                <li>PLC programming and maintenance.</li>
                <li>Rectifiers maintenance.</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </section><!-- /Resume Section -->

    <!-- Services Section -->
    <section id="services" class="services section">
      <div class="container section-title glowing-circle" data-aos="fade-up">
        <h2>AI Services</h2>
        <p>Comprehensive AI services for growth and innovation.</p>
      </div>

      <div class="container">
        <div class="row gy-4">
          <div class="col-lg-4 col-md-6" data-aos="fade-up" data-aos-delay="100">
            <div class="service-item">
              <!-- Icon removed from here -->
              <div>
                <h4 class="title"><a href="#" class="stretched-link" data-service-title="Generative AI & LLM Development" data-service-details="Building and deploying custom LLM-powered systems, including fine-tuning, RAG, and scalable chatbot applications with multilingual support. This involves architecting solutions that leverage the latest advancements in natural language processing and generative models to create intelligent and dynamic conversational agents and content generation tools.">GenAI & LLM Dev</a></h4>
                <p class="description">Custom LLM systems, fine-tuning, RAG, scalable multilingual chatbots.</p>
              </div>
            </div>
          </div>
          <div class="col-lg-4 col-md-6" data-aos="fade-up" data-aos-delay="200">
            <div class="service-item">
              <!-- Icon removed from here -->
              <div>
                <h4 class="title"><a href="#" class="stretched-link" data-service-title="Machine Learning & Deep Learning" data-service-details="Designing and implementing advanced ML/DL models for predictive analytics, computer vision, and NLP, including recommendation systems for hyper-personalization. My approach focuses on building robust, high-performance models that extract valuable insights from complex data and automate decision-making processes.">ML & Deep Learning</a></h4>
                <p class="description">Predictive analytics, computer vision, NLP, hyper-personalization.</p>
              </div>
            </div>
          </div>
          <div class="col-lg-4 col-md-6" data-aos="fade-up" data-aos-delay="300">
            <div class="service-item">
              <!-- Icon removed from here -->
              <div>
                <h4 class="title"><a href="#" class="stretched-link" data-service-title="Data Science & Analytics" data-service-details="Extracting insights from complex datasets, performing statistical analysis, and creating data-driven strategies. I specialize in transforming raw data into actionable intelligence, building compelling dashboards, and identifying key trends that inform business decisions.">Data Science & Analytics</a></h4>
                <p class="description">Insights from complex data, statistical analysis, data-driven strategies.</p>
              </div>
            </div>
          </div>
          <div class="col-lg-4 col-md-6" data-aos="fade-up" data-aos-delay="400">
            <div class="service-item">
              <!-- Icon removed from here -->
              <div>
                <h4 class="title"><a href="#" class="stretched-link" data-service-title="AI Strategy & Consulting" data-service-details="Guiding businesses on AI adoption, identifying opportunities, and developing roadmaps for AI integration, leveraging experience with foundational models. I help organizations navigate the AI landscape, from initial concept to full-scale implementation, ensuring a strategic and impactful approach.">AI Strategy & Consulting</a></h4>
                <p class="description">Guidance on AI adoption, opportunity identification, roadmap development.</p>
              </div>
            </div>
          </div>
          <div class="col-lg-4 col-md-6" data-aos="fade-up" data-aos-delay="500">
            <div class="service-item">
              <!-- Icon removed from here -->
              <div>
                <h4 class="title"><a href="#" class="stretched-link" data-service-title="Ethical AI & Responsible Deployment" data-service-details="Ensuring fairness, transparency, and accountability in AI systems, and implementing bias detection and mitigation techniques. My focus is on building AI solutions that are not only powerful but also responsible, addressing ethical considerations from design to deployment.">Ethical AI & Deployment</a></h4>
                <p class="description">Ensuring fairness, transparency, accountability; bias detection/mitigation.</p>
              </div>
            </div>
          </div>
          <div class="col-lg-4 col-md-6" data-aos="fade-up" data-aos-delay="600">
            <div class="service-item">
              <!-- Icon removed from here -->
              <div>
                <h4 class="title"><a href href="#" class="stretched-link" data-service-title="Cloud AI Integration & MLOps" data-service-details="Leveraging cloud platforms (AWS, Azure, GCP) for scalable AI model deployment, infrastructure, and MLOps pipelines. I facilitate seamless integration of AI models into existing cloud environments, ensuring efficient development, deployment, and monitoring of machine learning workflows.">Cloud AI & MLOps</a></h4>
                <p class="description">Scalable AI model deployment, infrastructure, MLOps pipelines.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section><!-- /Services Section -->

    <!-- Testimonials Section -->
    <section id="testimonials" class="testimonials section light-background">
      <div class="container section-title glowing-circle" data-aos="fade-up">
        <h2>Client Testimonials</h2>
        <p>What clients say about my AI solutions.</p>
      </div>

      <div class="container" data-aos="fade-up" data-aos-delay="100">
        <div class="swiper init-swiper">
          <script type="application/json" class="swiper-config">
            {
              "loop": true,
              "speed": 600,
              "autoplay": {
                "delay": 5000
              },
              "slidesPerView": "auto",
              "pagination": {
                "el": ".swiper-pagination",
                "type": "bullets",
                "clickable": true
              },
              "breakpoints": {
                "320": {
                  "slidesPerView": 1,
                  "spaceBetween": 40
                },
                "1200": {
                  "slidesPerView": 3,
                  "spaceBetween": 1
                }
              }
            }
          </script>
          <div class="swiper-wrapper">
            <div class="swiper-slide">
              <div class="testimonial-item">
                <p>
                  <i class="bi bi-quote quote-icon-left"></i>
                  <span>"Clayton developed multilingual chatbots leveraging LLMs, reducing contact center traffic."</span>
                  <i class="bi bi-quote quote-icon-right"></i>
                </p>
                <!-- Image removed as requested -->
                <h3>Learnmore Masanga</h3>
                <h4>GM AI | Mobile Telecom</h4>
              </div>
            </div>
            <div class="swiper-slide">
              <div class="testimonial-item">
                <p>
                  <i class="bi bi-quote quote-icon-left"></i>
                  <span>"His foundational models expertise led to hyper-personalization systems, growing customer numbers and revenue."</span>
                  <i class="bi bi-quote quote-icon-right"></i>
                </p>
                <!-- Image removed as requested -->
                <h3>Yvonne Kuimba</h3>
                <h4>Manager, Product Development</h4>
              </div>
            </div>
            <div class="swiper-slide">
              <div class="testimonial-item">
                <p>
                  <i class="bi bi-quote quote-icon-left"></i>
                  <span>"Clayton's expertise in AI transformed our data analytics, providing unprecedented insights."</span>
                  <i class="bi bi-quote quote-icon-right"></i>
                </p>
                <!-- Image removed as requested -->
                <h3>Trever Muchenje</h3>
                <h4>CTO, Data Innovations</h4>
              </div>
            </div>
            <div class="swiper-slide">
              <div class="testimonial-item">
                <p>
                  <i class="bi bi-quote quote-icon-left"></i>
                  <span>"The deep learning solution Clayton architected was groundbreaking; his innovative approach is exceptional."</span>
                  <i class="bi bi-quote quote-icon-right"></i>
                </p>
                <!-- Image removed as requested -->
                <h3>Freddy Chimire</h3>
                <h4>Lead AI Architect</h4>
              </div>
            </div>
            <div class="swiper-slide">
              <div class="testimonial-item">
                <p>
                  <i class="bi bi-quote quote-icon-left"></i>
                  <span>"Working with Clayton on our LLM project was a game-changer; highly effective conversational AI."</span>
                  <i class="bi bi-quote quote-icon-right"></i>
                </p>
                <!-- Image removed as requested -->
                <h3>Pamhidzai Mhembere</h3>
                <h4>Head of AI Strategy</h4>
              </div>
            </div>
            <div class="swiper-slide">
              <div class="testimonial-item">
                <p>
                  <i class="bi bi-quote quote-icon-left"></i>
                  <span>"Clayton's strategic insights into AI adoption were invaluable, ensuring powerful and responsible solutions."</span>
                  <i class="bi bi-quote quote-icon-right"></i>
                </p>
                <!-- Image removed as requested -->
                <h3>Michael Brown</h3>
                <h4>Director of Innovation</h4>
              </div>
            </div>
            <div class="swiper-slide">
              <div class="testimonial-item">
                <p>
                  <i class="bi bi-quote quote-icon-left"></i>
                  <span>"His expertise in optimizing ML pipelines significantly boosted our operational efficiency."</span>
                  <i class="bi bi-quote quote-icon-right"></i>
                </p>
                <!-- Image removed as requested -->
                <h3>Sarah Green</h3>
                <h4>Lead Data Scientist</h4>
              </div>
            </div>
          </div>
          <div class="swiper-pagination"></div>
        </div>
      </div>
    </section><!-- /Testimonials Section -->

    <!-- Contact Section -->
    <section id="contact" class="contact section">
      <div class="container section-title glowing-circle" data-aos="fade-up">
        <h2>Contact Me</h2>
        <p>Discuss your AI project or collaboration.</p>
        <p>Call me on <a href="tel:641-819-1309">641-819-1309</a></p>
      </div>

      <div class="container" data-aos="fade-up" data-aos-delay="100">
        <div class="row gy-4">
          <div class="col-lg-5">
            <div class="info-wrap">
              <div class="info-item d-flex" data-aos="fade-up" data-aos-delay="200">
                <i class="bi bi-geo-alt flex-shrink-0"></i>
                <div>
                  <h3>Global Presence</h3>
                  <p>Fairfield, Iowa, 52556</p>
                </div>
              </div>
              <div class="info-item d-flex" data-aos="fade-up" data-aos-delay="300">
                <i class="bi bi-telephone flex-shrink-0"></i>
                <div>
                  <h3>Call Me</h3>
                  <p><a href="tel:641-819-1309">641-819-1309</a></p>
                </div>
              </div>
              <div class="info-item d-flex" data-aos="fade-up" data-aos-delay="400">
                <i class="bi bi-envelope flex-shrink-0"></i>
                <div>
                  <h3>Email Me</h3>
                  <p><a href="mailto:csgwava@gmail.com">csgwava@gmail.com</a></p>
                </div>
              </div>
              <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d15313.238478479538!2d31.0253457!3d-17.8286786!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x1931a54160408581%3A0x6b771e3d3b7a5a8f!2sHarare%2C%20Zimbabwe!5e0!3m2!1sen!2sus!4v1700000000000!5m2!1sen!2sus" frameborder="0" style="border:0; width: 100%; height: 270px;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
            </div>
          </div>

          <div class="col-lg-7">
            <form action="https://formspree.io/f/xgvyoapn" method="POST" class="php-email-form" data-aos="fade-up" data-aos-delay="200">
              <div class="row gy-4">
                <div class="col-md-6">
                  <label for="name-field" class="pb-2">Your Name</label>
                  <input type="text" name="name" id="name-field" class="form-control" required>
                </div>
                <div class="col-md-6">
                  <label for="email-field" class="pb-2">Your Email</label>
                  <input type="email" class="form-control" name="email" id="email-field" required>
                </div>
                <div class="col-md-12">
                  <label for="subject-field" class="pb-2">Subject</label>
                  <input type="text" class="form-control" name="subject" id="subject-field" required>
                </div>
                <div class="col-md-12">
                  <label for="message-field" class="pb-2">Message</label>
                  <textarea class="form-control" name="message" rows="10" id="message-field" required></textarea>
                </div>
                <div class="col-md-12 text-center">
                  <div class="loading">Loading</div>
                  <div class="error-message"></div>
                  <div class="sent-message">Your message has been sent. Thank you!</div>
                  <button type="submit">Send Message</button>
                </div>
              </div>
            </form>

          </div>
        </div>
      </div>
    </section><!-- /Contact Section -->

  </main>

  <!-- Service Details Modal Overlay -->
  <div id="serviceDetailsModal" class="service-details-modal-overlay">
    <div class="service-details-modal-content">
      <button id="closeServiceModalBtn" class="close-btn">&times;</button>
      <h3 id="modalServiceTitle"></h3>
      <p id="modalServiceDetails"></p>
    </div>
  </div>

  <!-- Certificate Details Modal Overlay (NEW) -->
  <div class="certificate-details-modal-overlay">
    <div class="certificate-details-modal-content">
      <button class="close-btn">&times;</button>
      <h3 id="modalCertificateTitle"></h3>
      <p id="modalCertificateDetails"></p>
      <a id="modalCertificateLink" href="#" target="_blank" class="btn btn-primary mt-3">View Certificate</a>
    </div>
  </div>

  <footer id="footer" class="footer position-relative">
    <div class="container">
      <div class="copyright text-center ">
        <p>© <span>Copyright</span> <strong class="px-1 sitename">Clayton Gwava</strong> <span>All Rights Reserved</span></p>
      </div>
    </div>
  </footer>

  <!-- Vendor JS Files -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" crossorigin="anonymous"></script>
  <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
  <script src="https://unpkg.com/typed.js@2.1.0/dist/typed.umd.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/@srexi/purecounterjs/dist/purecounter_vanilla.js"></script>
  <script src="https://cdn.jsdelivr.net/gh/mcstudios/glightbox/dist/js/glightbox.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
  <script src="https://unpkg.com/imagesloaded@5/imagesloaded.pkgd.min.js"></script>
  <script src="https://unpkg.com/isotope-layout@3/dist/isotope.pkgd.min.js"></script>

  <!-- Main JS File -->
  <script>
    document.addEventListener('DOMContentLoaded', () => {
      "use strict";

      /**
       * Preloader
       * Removes the preloader once the entire page has loaded.
       */
      const preloader = document.querySelector('#preloader');
      if (preloader) {
        window.addEventListener('load', () => {
          preloader.remove();
        });
      }

      /**
       * Scroll top button
       * Shows/hides a scroll-to-top button based on scroll position.
       */
      let scrollTop = document.querySelector('.scroll-top');

      function toggleScrollTop() {
        if (scrollTop) {
          window.scrollY > 100 ? scrollTop.classList.add('active') : scrollTop.classList.remove('active');
        }
      }
      window.addEventListener('load', toggleScrollTop);
      document.addEventListener('scroll', toggleScrollTop);
      if (scrollTop) {
        scrollTop.addEventListener('click', (e) => {
          e.preventDefault();
          window.scrollTo({
            top: 0,
            behavior: 'smooth'
          });
        });
      }

      /**
       * Mobile Navigation Toggle
       */
      const mobileNavToggle = document.querySelector('.mobile-nav-toggle');
      const mobileNav = document.querySelector('.mobile-nav');
      const logoContainer = document.querySelector('.logo-container'); // Get the logo container

      if (mobileNavToggle && mobileNav) {
        mobileNavToggle.addEventListener('click', (e) => {
          mobileNav.classList.toggle('active');
          mobileNavToggle.classList.toggle('bi-list');
          mobileNavToggle.classList.toggle('bi-x'); // Change icon to 'x' when active

          // Toggle logo visibility
          if (window.innerWidth <= 768) { // Only apply on mobile
            if (mobileNav.classList.contains('active')) {
              logoContainer.style.display = 'none'; // Hide logo
            } else {
              logoContainer.style.display = 'block'; // Show logo
            }
          }
        });

        // Close mobile nav when clicking on a link
        mobileNav.querySelectorAll('a.scrollto').forEach(link => {
          link.addEventListener('click', () => {
            mobileNav.classList.remove('active');
            mobileNavToggle.classList.remove('bi-x');
            mobileNavToggle.classList.add('bi-list');
            if (window.innerWidth <= 768) { // Only apply on mobile
              logoContainer.style.display = 'block'; // Show logo when nav closes
            }
          });
        });

        // Ensure logo is visible on resize if not in mobile nav view
        window.addEventListener('resize', () => {
          if (window.innerWidth > 768) {
            logoContainer.style.display = 'block'; // Always show logo on desktop
          } else if (!mobileNav.classList.contains('active')) {
            logoContainer.style.display = 'block'; // Show logo on mobile if nav is closed
          }
        });
      }


      /**
       * Animation on scroll function and init (AOS)
       * Initializes the AOS library for scroll animations.
       */
      function aosInit() {
        AOS.init({
          duration: 600,
          easing: 'ease-in-out',
          once: true,
          mirror: false
        });
      }
      window.addEventListener('load', aosInit);

      /**
       * Init typed.js
       * Initializes the Typed.js library for dynamic text typing effects.
       */
      const selectTyped = document.querySelector('.typed');
      if (selectTyped) {
        let typed_strings = selectTyped.getAttribute('data-typed-items');
        typed_strings = typed_strings.split(',');
        new Typed('.typed', {
          strings: typed_strings,
          loop: true,
          typeSpeed: 100,
          backSpeed: 50,
          backDelay: 2000
        });
      }

      /**
       * Initiate Pure Counter
       * Initializes the PureCounter library for animated number counting.
       */
      new PureCounter();

      /**
       * Animate the skills items on reveal
       * Triggers skill bar animations when the skills section comes into view.
       */
      let skillsSection = document.querySelector('#skills');
      if (skillsSection) {
        const animateSkills = () => {
          let progressBars = document.querySelectorAll('.skills-content .progress-bar');
          progressBars.forEach((el) => {
            el.style.width = el.getAttribute('aria-valuenow') + '%';
          });
        };

        const checkSkillsVisibility = () => {
          if (skillsSection.getBoundingClientRect().top < window.innerHeight * 0.8 && skillsSection.getBoundingClientRect().bottom > 0) {
            animateSkills();
            // Optional: remove event listener once animated to prevent re-animation
            // window.removeEventListener('scroll', checkSkillsVisibility);
          }
        };

        // Check on load and on scroll
        window.addEventListener('scroll', checkSkillsVisibility);
        window.addEventListener('load', checkSkillsVisibility);
      }

      /**
       * Initiate glightbox
       * Initializes the GLightbox library for responsive image/video lightboxes.
       */
      const glightbox = GLightbox({
        selector: '.glightbox'
      });

      /**
       * Init isotope layout and filters
       * Initializes Isotope.js for dynamic grid layouts and filtering.
       */
      document.querySelectorAll('.ai-isotope-layout').forEach(function(isotopeItem) {
        let layout = isotopeItem.getAttribute('data-layout') ?? 'masonry';
        let filter = isotopeItem.getAttribute('data-default-filter') ?? '*';
        let sort = isotopeItem.getAttribute('data-sort') ?? 'original-order';

        let initIsotope;
        if (typeof imagesLoaded !== 'undefined' && typeof Isotope !== 'undefined') {
          imagesLoaded(isotopeItem.querySelector('.ai-isotope-container'), function() {
            initIsotope = new Isotope(isotopeItem.querySelector('.ai-isotope-container'), {
              itemSelector: '.ai-portfolio-item',
              layoutMode: layout,
              filter: filter,
              sortBy: sort
            });
          });

          isotopeItem.querySelectorAll('.ai-portfolio-filters li').forEach(function(filters) {
            filters.addEventListener('click', function() {
              isotopeItem.querySelector('.ai-portfolio-filters .ai-filter-active').classList.remove('ai-filter-active');
              this.classList.add('ai-filter-active');
              initIsotope.arrange({
                filter: this.getAttribute('data-filter')
              });
              if (typeof aosInit === 'function') {
                aosInit();
              }
            }, false);
          });
        } else {
          console.warn("Isotope.js or imagesLoaded.js not found. Portfolio filtering may not work as expected.");
        }
      });

      /**
       * Init swiper sliders
       * Initializes Swiper.js for carousels and sliders.
       */
      function initSwiper() {
        document.querySelectorAll(".init-swiper").forEach(function(swiperElement) {
          let config = JSON.parse(
            swiperElement.querySelector(".swiper-config").innerHTML.trim()
          );
          new Swiper(swiperElement, config);
        });
      }
      window.addEventListener("load", initSwiper);

      /**
       * Correct scrolling position upon page load for URLs containing hash links.
       * Ensures smooth scroll to the correct section if a hash is present in the URL.
       */
      window.addEventListener('load', function(e) {
        if (window.location.hash) {
          if (document.querySelector(window.location.hash)) {
            setTimeout(() => {
              let section = document.querySelector(window.location.hash);
              window.scrollTo({
                top: section.offsetTop,
                behavior: 'smooth'
              });
            }, 100);
          }
        }
      });

      /**
       * Main Navigation Scrollspy (for desktop only)
       * Highlights the active navigation link based on the current scroll position.
       */
      let mainNavLinks = document.querySelectorAll('#main-nav a.scrollto');

      function mainNavScrollspy() {
        if (window.innerWidth <= 768) return; // Only for desktop

        const sections = document.querySelectorAll('section');
        let currentActiveSectionId = null;

        sections.forEach(section => {
          if (!section.id) return;

          const sectionTop = section.offsetTop - 70; // Adjust for fixed header
          const sectionHeight = section.offsetHeight;
          const scrollPosition = window.scrollY;

          if (scrollPosition >= sectionTop && scrollPosition < (sectionTop + sectionHeight)) {
            currentActiveSectionId = section.id;
          }
        });

        mainNavLinks.forEach(navlink => {
          if (navlink.hash && navlink.hash.substring(1) === currentActiveSectionId) {
            navlink.classList.add('active');
          } else {
            navlink.classList.remove('active');
          }
        });
      }
      window.addEventListener('load', mainNavScrollspy);
      document.addEventListener('scroll', mainNavScrollspy);


      /**
       * Service Details Modal Logic
       */
      const serviceDetailsModal = document.getElementById('serviceDetailsModal');
      const modalServiceTitle = document.getElementById('modalServiceTitle');
      const modalServiceDetails = document.getElementById('modalServiceDetails');
      const serviceItems = document.querySelectorAll('.services .service-item .stretched-link');
      const closeServiceModalBtn = document.getElementById('closeServiceModalBtn'); // Get the close button

      serviceItems.forEach(item => {
        item.addEventListener('click', function(event) {
          event.preventDefault(); // Prevent default link behavior
          const title = this.getAttribute('data-service-title');
          const details = this.getAttribute('data-service-details');
          openServiceDetailsModal(title, details);
        });
      });

      // Event listener for the close button
      if (closeServiceModalBtn) {
        closeServiceModalBtn.addEventListener('click', () => {
          closeServiceDetailsModal();
        });
      }

      function openServiceDetailsModal(title, details) {
        modalServiceTitle.textContent = title;
        modalServiceDetails.textContent = details;
        serviceDetailsModal.classList.add('active');
        document.body.classList.add('no-scroll'); // Disable body scroll
      }

      function closeServiceDetailsModal() {
        serviceDetailsModal.classList.remove('active');
        document.body.classList.remove('no-scroll'); // Enable body scroll
      }

      // Close modal when clicking outside content
      serviceDetailsModal.addEventListener('click', function(event) {
        if (event.target === serviceDetailsModal) {
          closeServiceDetailsModal();
        }
      });

      // Close modal with Escape key
      document.addEventListener('keydown', function(event) {
        if (event.key === 'Escape' && serviceDetailsModal.classList.contains('active')) {
          closeServiceModalBtn.click(); // Programmatically click the close button
        }
      });


      /**
       * Theme Toggle Logic
       * Allows users to switch between light and dark modes, and persists the choice.
       */
      const themeToggleBtn = document.getElementById('themeToggle');
      const sunIcon = themeToggleBtn ? themeToggleBtn.querySelector('.bi-sun') : null;
      const moonIcon = themeToggleBtn ? themeToggleBtn.querySelector('.bi-moon') : null;

      // Function to apply the theme based on the current state or localStorage
      function applyTheme(theme) {
        if (theme === 'dark') {
          document.body.classList.add('dark-mode');
          if (sunIcon) sunIcon.style.display = 'none';
          if (moonIcon) moonIcon.style.display = 'inline-block';
        } else {
          document.body.classList.remove('dark-mode');
          if (sunIcon) sunIcon.style.display = 'inline-block';
          if (moonIcon) moonIcon.style.display = 'none';
        }
      }

      // Check for saved theme on page load
      const savedTheme = localStorage.getItem('theme');
      if (savedTheme) {
        applyTheme(savedTheme);
      } else {
        // Default to light mode if no theme is saved
        applyTheme('light');
      }

      // Add event listener to the theme toggle button
      if (themeToggleBtn) {
        themeToggleBtn.addEventListener('click', () => {
          if (document.body.classList.contains('dark-mode')) {
            applyTheme('light');
            localStorage.setItem('theme', 'light');
          } else {
            applyTheme('dark');
            localStorage.setItem('theme', 'dark');
          }
        });
      }


      /**
       * Certificates Carousel and Details Modal Logic (NEW)
       */
      // Initialize Swiper for Certificates Carousel
      new Swiper('.certificates-carousel', {
        speed: 600,
        loop: true,
        autoplay: {
          delay: 5000,
          disableOnInteraction: false
        },
        slidesPerView: 'auto',
        pagination: {
          el: '.swiper-pagination',
          type: 'bullets',
          clickable: true
        },
        breakpoints: {
          320: {
            slidesPerView: 1,
            spaceBetween: 20
          },
          576: {
            slidesPerView: 2,
            spaceBetween: 20
          },
          768: {
            slidesPerView: 3,
            spaceBetween: 30
          },
          992: {
            slidesPerView: 4,
            spaceBetween: 30
          }
        }
      });

      const certificateModalOverlay = document.querySelector('.certificate-details-modal-overlay');
      const closeCertificateModalBtn = document.querySelector('.certificate-details-modal-content .close-btn');
      const modalCertificateTitle = document.getElementById('modalCertificateTitle');
      const modalCertificateDetails = document.getElementById('modalCertificateDetails');
      const modalCertificateLink = document.getElementById('modalCertificateLink');

      // Populate with real certificate data (replace placeholders)
      const certificatesData = {
        cert1: {
          title: 'Google Professional ML Engineer',
          details: 'Certified by Google Cloud, this validates my expertise in designing, building, and productionizing machine learning models using Google Cloud technologies. Focuses on MLOps best practices.',
          link: 'https://tinyurl.com/ycu33t9k' // Updated link
        },
        cert2: {
          title: 'TOGAF 9 Practitioner',
          details: 'The Open Group Architecture Framework (TOGAF) certification confirms my understanding of enterprise architecture, enabling me to design and implement robust IT solutions aligned with business strategy.',
          link: 'https://tinyurl.com/yvyvxmm9' // Updated link
        },
        cert3: {
          title: 'PRINCE2 Agile Practitioner',
          details: 'PRINCE2 Agile is a blend of PRINCE2 project management and agile methodologies, certifying my ability to manage complex projects with flexibility and adaptability.',
          link: 'https://tinyurl.com/y78umwnw' // Updated link
        },
        cert4: {
          title: 'Applied Data Science 1',
          details: 'This course provides foundational knowledge and practical skills in applied data science, covering key techniques for data manipulation, analysis, and interpretation.',
          link: 'https://tinyurl.com/u763aacs' // Added link
        },
        cert5: {
          title: 'Machine Learning Specialization',
          details: 'This specialization from DeepLearning.AI and Coursera covers fundamental machine learning concepts, algorithms, and practical applications, including supervised and unsupervised learning. It was a foundational course for my ML journey.',
          link: 'https://www.coursera.org/verify/YOUR_ML_CERT_ID_PLACEHOLDER'
        },
        cert6: {
          title: 'Generative AI with Transformers',
          details: 'An advanced course from Hugging Face on Coursera, focusing on the latest in generative AI models, particularly Transformers, and their practical applications in natural language processing and content creation.',
          link: 'https://www.coursera.org/verify/YOUR_GENAI_CERT_ID_PLACEHOLDER'
        },
        cert7: {
          title: 'Deep Learning Specialization',
          details: 'A cornerstone specialization from DeepLearning.AI on Coursera, providing comprehensive knowledge of neural networks, convolutional networks, recurrent networks, and the practical aspects of building deep learning models.',
          link: 'https://www.coursera.org/verify/YOUR_DL_CERT_ID_PLACEHOLDER'
        },
        cert8: {
          title: 'Reinforcement Learning',
          details: 'This course from the University of Alberta on Coursera introduces the core concepts of reinforcement learning, including Markov Decision Processes, value functions, and policy gradient methods for training intelligent agents.',
          link: 'https://www.coursera.org/verify/YOUR_RL_CERT_ID_PLACEHOLDER'
        },
        cert9: {
          title: 'Cisco Cybersecurity',
          details: 'This Cisco Networking Academy course equipped me with fundamental knowledge in cybersecurity, including threat detection, network security, and incident response.',
          link: 'https://www.netacad.com/credentials/YOUR_CISCO_CYBER_ID_PLACEHOLDER'
        },
        cert10: {
          title: 'Linux Essentials',
          details: 'Covering fundamental Linux concepts and commands, this Cisco Networking Academy certificate is crucial for working with server environments and development tools.',
          link: 'https://www.netacad.com/credentials/YOUR_CISCO_LINUX_ID_PLACEHOLDER'
        },
        cert11: {
          title: 'Mobility Fundamental',
          details: 'This Cisco Networking Academy course provides an understanding of wireless networking, mobile technologies, and their implications for modern communication systems.',
          link: 'https://www.netacad.com/credentials/YOUR_CISCO_MOBILITY_ID_PLACEHOLDER'
        },
        cert12: {
          title: 'Scientific Computing & Python for Data Science',
          details: 'From WorldQuant University, this course enhanced my Python skills for numerical computing, data manipulation, statistical analysis, and data visualization, essential for data science roles.',
          link: 'https://www.worldquantuniversity.org/certificate/YOUR_WQ_PYTHON_ID_PLACEHOLDER'
        }
      };

      document.querySelectorAll('.certificate-item').forEach(item => {
        item.addEventListener('click', () => {
          const certId = item.dataset.certificateId;
          const cert = certificatesData[certId];
          if (cert) {
            modalCertificateTitle.textContent = cert.title;
            modalCertificateDetails.textContent = cert.details;
            modalCertificateLink.href = cert.link;
            certificateModalOverlay.classList.add('active');
            document.body.classList.add('no-scroll'); // Disable background scroll
          }
        });
      });

      closeCertificateModalBtn.addEventListener('click', () => {
        certificateModalOverlay.classList.remove('active');
        document.body.classList.remove('no-scroll'); // Re-enable background scroll
      });

      certificateModalOverlay.addEventListener('click', (e) => {
        if (e.target === certificateModalOverlay) {
          certificateModalOverlay.classList.remove('active');
          document.body.classList.remove('no-scroll');
        }
      });
    });
  </script>
</body>

</html>
