<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Valentine 💖</title>
<style>
body {
    margin: 0;
    font-family: 'Arial', sans-serif;
    background: linear-gradient(135deg, #ff9a9e, #fad0c4);
    text-align: center;
    color: #fff;
}

.page {
    display: none;
    padding: 20px;
    min-height: 100vh;
}

.active {
    display: block;
}

h1 {
    font-size: 28px;
    margin-top: 20px;
}

.photos img {
    width: 90%;
    max-width: 250px;
    margin: 10px;
    border-radius: 15px;
    box-shadow: 0 8px 20px rgba(0,0,0,0.3);
}

button {
    padding: 12px 25px;
    font-size: 18px;
    border: none;
    border-radius: 25px;
    margin: 10px;
    cursor: pointer;
}

.yes {
    background: #ff4d6d;
    color: white;
}

.no {
    background: #444;
    color: white;
}

.message-box {
    background: rgba(0,0,0,0.4);
    padding: 20px;
    border-radius: 20px;
    margin: 20px;
}

.bg-love {
    background: url('photo3.jpg') center/cover no-repeat;
}
</style>
</head>

<body>

<!-- PAGE 1 -->
<div class="page active" id="page1">
    <div class="photos">
        <img src="photo1.jpg">
        <img src="photo2.jpg">
        <img src="photo3.jpg">
    </div>

    <h1>Will you be my Valentine,<br>RECHA Maharani? 💐</h1>

    <button class="yes" onclick="goYes()">YES 💗</button>
    <button class="no" onclick="goNo()">NO 😶</button>
</div>

<!-- PAGE NO -->
<div class="page" id="pageNo">
    <h1>Eh… really? 🥺</h1>
    <p>Think again…</p>
    <p>Don’t do this 😭</p>
    <p><strong>Please choose YES, sanu 💗</strong></p>

    <button class="yes" onclick="goYes()">OKAY, YES 😌</button>
</div>

<!-- PAGE YES -->
<div class="page bg-love" id="pageYes">
    <div class="message-box">
        <p>
        I just want you to know how grateful I am for you—<br>
        <i>(tara timi malaie maya gardaineu)</i><br><br>

        You’re not just someone I love,<br>
        you’re the one whom I love you most,<br>
        and grateful for every single day.<br><br>

        Your love is my comfort,<br>
        and my love for you is real, deep,<br>
        and forever kind of love.<br><br>

        You know how much I love you…<br>
        and I always will 💗<br><br>

        <i>(Chito vetam na lastai maya lacha 🥹)</i>
        </p>
    </div>
</div>

<script>
function goNo() {
    document.getElementById("page1").classList.remove("active");
    document.getElementById("pageNo").classList.add("active");
}

function goYes() {
    document.getElementById("page1").classList.remove("active");
    document.getElementById("pageNo").classList.remove("active");
    document.getElementById("pageYes").classList.add("active");
}
</script>

</body>
</html>
