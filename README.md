<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viemport" content="width, initial-scare=1.0">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap" rel="stylesheet">
<link rel="stylesheet" href=https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/css/all.min.css>
<link rel="stylesheet" href="./style.css">
<title> Stylish Profile Card</title>
</head>
<body>
<div class="profile-container">
<div class="img-container">
<img src="https://i.mycdn.me/i?r=BDHElZJBPNKGuFyY-akIDfgnPy87SpywPGUcveTTTWmFX_1Dfhbk5kSAw9GisWfhXMs" alt="profile image">
</div>
<p class="info full-name">Kosyrkov Nikita</p>
<p class="info role">
<i class="fas fa-star"></i>
UX/UI Developer
</p>
<p class="info plase">
<i class="fas fa-map-marker-alt"></i>
Moscow, Russia
</p>
<div class="posts-info">
    <p><span>336</span> Posts</p>
    <p><span>4300</span> Likes</p>
    <p><span>87</span> Works</p>
</div>

<div class="social-container">
    <button class="youtube">
        <i class="fab fa-youtube"></i>
    </button>
    <button class="linkedin">
        <i class="fab fa-linkedin"></i>
    </button>
    <button class="instagram">
        <i class="fab fa-instagram"></i>
    </button>
    <button class="github">
        <i class="fab fa-github"></i>
    </button>
</div>
<button class="action">Follow</button>
<button class="action message">message</button>
</div>
</body>
</html>


* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    color: #334e64;
    font-family: "Montserrat", sans-serif;
}

body {
    min-height: 100vh;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(20deg, #ff2844,#6741ff);
}

.profile-container {
    position: relative;
    background-color: #ffffff;
    width: 350px;
    padding: 100px 50px 40px;
    border-radius: 12px;
    box-shadow: 0 0 60px 5px rgba(0, 0, 0 0.2);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.img-container{
    width: 130px;
    height: 130px;
    overflow: hidden;
    border: 5px solid #b92a76;
    border-radius: 50%;
    box-shadow: 0 8px 55px #b92a76a4;
    position: absolute;
    top: 0;
    left: 50%;
    transform: translate(-50%, -50%);
}

.img-container img {
    width: 100%;
    max-width: 100%;
    transform: scale(1.1);
}

.info {
    margin-bottom: 12px;
}

.info i {
    margin-right: 8px;
    font-size: 1.1em;
}

.place{
    margin-bottom: 40px;
}

.full-name {
    font-size: 1.4em;
    font-weight: bold;
    letter-spacing: 1px;
    color: #b92a76;
}

.posts-info {
    width: 100%;
    display: flex;
    justify-content: space-around;
    align-items: center;
    font-size: 1.1em;
    letter-spacing: 0.5px;
    margin-bottom: 30px;
    text-align: center;
}

.posts-info span {
    display: block;
    font-weight: bold;
    margin-bottom: 4px;
}

.social-container {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}

.social-container i {
    color: #ffffff;
}

.social-container button {
    border: none;
    outline: none;
    width: 45px;
    height: 45px;
    border-radius: 50%;
    font-size: 1.2em;
    cursor: pointer;
    box-shadow: 0px 5px 25px rgba(0, 0, 0, 0.15);
    transition: transform 0.3s;
}

.social-container button:hover {
    transform: scale(1.1);
}

/* Social colors */

.social-container button.youtube {
    background: linear-gradient(45deg, #ff000088, #ff0000);
}

.social-container button.linkedin {
    background: linear-gradient(45deg, #0e76a888, #0e76a8);
}

.social-container button.instagram {
    background: linear-gradient(45deg, #e6683ccc 25%, #dc2743 50%);
}

.social-container button.github {
    background: linear-gradient(45deg, #33333388, #333333);
}

.action {
    outline: none;
    cursor: pointer;
    color: #ffffff;
    background-color: #d31258;
    border: none;
    border-radius: 50px;
    padding: 12px 20px;
    width: 80%;
    margin-top: 25px;
    box-shadow: 0px 8px 25px rgba(0, 0, 0 0.2);
    text-transform: uppercase;
    font-size: lem;
    font-weight: bold;
    letter-spacing: 2px;
    transition: transform 0.3s;
}

.action.message {
    background-color: #6741ff;
}

.action:hover {
    transform: scale(1.05);
    opacity: 0.85;
}
