body {
    font-family: 'Roboto', sans-serif;
    color: white;
    background-color: black;
    margin: 0;
}

body.light-mode {
    background: white;
    color: black;
}



/* Navigator */


#sticky-bar {
    position: sticky;
    top: 0;
    width: 100%;
    background-color: #222;
    display: flex;
    padding: 0.5rem 1rem;
    border-bottom: 2px solid #333;
    z-index: 1;
}

.light-mode #sticky-bar {
    color: black;
    background-color: white;
    border-bottom: none;
}

#link-container {
    gap: 1.5rem;
    flex-wrap: wrap;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: rgba(0, 0, 0, 0.8);
    padding: 10px 20px;
}

.light-mode #link-container {
    background-color: #c3c3c3;
}

#link-container a {
    text-decoration: none;
    color: #fff;
    margin: 0 10px;
    font-size: 16px;
    transition: color 0.3s ease-in-out;
}

.light-mode #link-container a {
    color: black;
}

#link-container a:hover {
    color: #ff6347;
}

a {
    padding: 1.5rem;
    color: white;
    text-decoration: none;
    font-weight: bold;
    transition: background-color 0.7s ease;
}

nav a {
    color: white;
    margin: 0 15px;
    font-weight: bold;
    position: relative;
    transition: color 0.3s;
}

nav a:hover {
    color: #ff6347;
}

nav a::after {
    content: ''; /* Adds a decorative line under the link */
    position: absolute;
    left: 0; /* Start from the left */
    bottom: -3px; /* Position below the text */
    height: 3px; /* Line height */
    width: 0; /* Initial width */
    background: #ff6347; /* Line color */
    transition: width 0.3s;
}

nav a:hover::after {
    width: 100%; /* Expands line to full width on hover */
}

.nav-search {
    border: none;
    border-radius: 4px;
    outline: none;
    font-size: 14px;
    height: 30px;
    background: #4e4e4e;
}

.light-mode .nav-search {
    color: black;
    background-color: #9e9e9e;
}

.dropdown {
    position: relative;
    display: inline-block;
}

.dropbtn {
    background-color: #444;
    color: white;
    padding: 8px 12px;
    font-size: 16px;
    border: none;
    cursor: pointer;
    border-radius: 4px;
    transition: background 0.3s;
}

.light-mode .dropbtn {
    background-color: #9e9e9e;
}

.dropbtn:hover {
    background-color: #666;
}

.dropdown-content {
    display: none;
    position: absolute;
    background-color: #333;
    min-width: 150px;
    box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.2);
    z-index: 1;
    border-radius: 4px;
}

.light-mode .dropdown-content {
    background-color: #666;
}

.dropdown-content a {
    color: white;
    padding: 10px 12px;
    text-decoration: none;
    display: block;
    font-size: 14px;
    border-bottom: 1px solid rgba(255, 255, 255, 0.2);
}

.dropdown-content a:hover {
    background-color: #575757;
}

.dropdown:hover .dropdown-content {
    display: block;
}

.theme-toggle {
    background-color: #ff4326;
    color: #fff;
    padding: 8px 15px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    transition: background 0.3s;
    font-size: 14px;
}

.theme-toggle:hover {
    background-color: #ff4326;
}






/* Animations */
@keyframes fadeInUp {
    from {
        transform: translateY(20px);
        opacity: 0;
    }
    to {
        transform: translateY(0);
        opacity: 1;
    }
}

@keyframes slideUp {
    from {
        transform: translateY(20px);
        opacity: 0;
    }
    to {
        transform: translateY(0);
        opacity: 1;
    }
}

@keyframes fadeInDown {
    from {
        transform: translateY(-100%);
        opacity: 0;
    }
    to {
        transform: translateY(0); /
        opacity: 1;
    }
}

@keyframes fadeIn {
    from {
        opacity: 0;
    }
    to {
        opacity: 1; 
    }
}






footer {
    text-align: center;
    padding: 20px;
    background: #1e1e1e;
    color: #fff;
    font-size: 14px;
}

.light-mode footer {
    color: black;
    background: #b8b8b8;
}

.social-links {
    margin-top: 10px;
    display: flex;
    justify-content: center;
    gap: 20px;
}

.social-links button {
    background-color: #555;
    color: #fff;
    border: none;
    padding: 10px;
    font-size: 16px;
    cursor: pointer;
    border-radius: 5px;
    transition: background-color 0.3s ease;
    display: flex;
    align-items: center;
    gap: 10px;
}

.social-links button:hover {
    background-color: #007bff;
}

.social-links img {
    width: 20px;
    height: 20px;
}
