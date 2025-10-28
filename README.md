Tosha Express Bus Booking Website
Overview

A modern, responsive bus booking website for Tosha Express built with HTML, CSS, Bootstrap 5, and JavaScript. The site allows users to search for bus routes across Kenya, select seats from an interactive seat map, and complete bookings via WhatsApp integration.
Project Structure

    index.html - Main bus booking page with booking form, route listings, and seat selection modal
    styles.css - Custom CSS styling for the bus booking theme including seat map interface
    IMG-20251017-WA0016.jpg - Favicon/icon image
    IMG-20251017-WA0015.jpg - Bus interior seats image
    IMG-20251017-WA0017.jpg - Route card image (Mombasa-Malindi)
    IMG-20251017-WA0018.jpg - Route card image (Nairobi-Kisumu)
    IMG-20251017-WA0019.jpg - Route card image (Nairobi-Mombasa)
    IMG-20251017-WA0021.jpg - Hero section background image

Technology Stack

    HTML5
    CSS3 with custom properties
    Bootstrap 5.0.1 (via CDN)
    Bootstrap Icons (via CDN)
    Vanilla JavaScript for form handling, seat selection, and WhatsApp integration

Features

    Booking Form: Route selection for Kenyan cities (Nairobi, Mombasa, Kisumu, Nakuru, Eldoret, Malindi, Kisii, Kakamega, Meru, Nyeri), date picker, and passenger count
    Interactive Seat Selection: Visual seat map with 32 seats (8 rows x 4 seats)
        Available seats (blue outline)
        Selected seats (blue fill)
        Booked seats (red, disabled)
        Aisle separation for realistic bus layout
    Popular Routes:
        Nairobi → Mombasa (8 hours, KSh 1,500)
        Nairobi → Kisumu (6 hours, KSh 1,200)
        Mombasa → Malindi (2 hours, KSh 600)
    Why Choose Us: Feature highlights with icons
    WhatsApp Integration: Booking completion redirects to WhatsApp with full details
    Responsive Design: Mobile-friendly layout with touch-optimized seat selection

Seat Selection Flow

    User fills out booking form (from, to, date, passengers)
    Modal opens with booking summary and interactive seat map
    User selects required number of seats (matching passenger count)
    WhatsApp button enables only when correct number of seats selected
    Click WhatsApp button to complete booking with seat numbers included

WhatsApp Integration

When users complete the booking form and select seats:

    A modal displays the booking summary and seat selection interface
    Users select their seats from the visual seat map
    Once seats are selected, the "Complete on WhatsApp" button becomes enabled
    They are redirected to WhatsApp with pre-filled booking details including:
        Route (from/to cities)
        Travel date
        Number of passengers
        Selected seat numbers
    WhatsApp number: +254 712 345 678
    Email: booking@toshaexpress.co.ke

Recent Changes

    2025-10-20: Rebranded from Swift Bus to Tosha Express
    Updated all routes to Kenyan long-distance destinations
    Replaced all images with custom Tosha Express photos
    Changed currency from USD to KSh (Kenyan Shilling)
    Updated WhatsApp contact to Kenyan format (+254)
    Added favicon using company icon
    Pricing adjusted for Kenyan market
    Initial setup from portfolio site to bus booking platform
    Implemented interactive seat selection with visual seat map
    Fixed seat selection reset bug to ensure proper state between bookings
    Added defensive validation in WhatsApp handler

Deployment

    Frontend runs on port 5000
    Uses Python's built-in HTTP server for serving static files
    Configured for autoscale deployment on Replit

Next Steps for Production

    Update WhatsApp phone number to actual Tosha Express number
    Add real-time route pricing and schedules
    Implement backend for real-time seat availability checking
    Connect to database for seat booking persistence
    Add M-Pesa payment integration for Kenya
    Implement user authentication for booking history
    Add SMS confirmation using Safaricom API
