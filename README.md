داخلا فارم ڀرڻ 
index.html
<!DOCTYPE html>
<html lang="sd" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GBELS Wassan | آفيشل ويب سائيٽ</title>
    <style>
        :root { --primary: #004d40; --secondary: #ffc107; --bg: #f4f7f6; }
        body { font-family: 'Segoe UI', Tahoma, sans-serif; margin: 0; padding: 0; background-color: var(--bg); text-align: center; color: #333; }
        header { background: var(--primary); color: white; padding: 40px; border-bottom: 8px solid var(--secondary); }
        nav { background: #242526; padding: 10px; position: sticky; top: 0; z-index: 1000; }
        nav a { color: white; text-decoration: none; padding: 10px 15px; font-weight: bold; }

        .container { max-width: 1000px; margin: auto; padding: 20px; }
        .card { background: white; padding: 25px; border-radius: 15px; box-shadow: 0 4px 10px rgba(0,0,0,0.1); margin-bottom: 30px; }
        
        .gallery { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; }
        .gallery img { width: 100%; border-radius: 10px; border: 3px solid #ddd; height: 200px; object-fit: cover; }

        .btn { display: inline-block; padding: 12px 25px; border-radius: 30px; text-decoration: none; font-weight: bold; margin: 10px; transition: 0.3s; }
        .btn-wa { background: #25d366; color: white; }
        .btn-map { background: var(--primary); color: white; }

        input { padding: 12px; border-radius: 5px; border: 1px solid #ccc; width: 60%; margin-bottom: 10px; }
        button { padding: 12px 25px; background: var(--primary); color: white; border: none; border-radius: 5px; cursor: pointer; }
        
        footer { background: #1c1e21; color: white; padding: 30px; margin-top: 50px; }
    </style>
</head>
<body>

<header>
    <h1>گورنمينٽ بوائز ايليمينٽري لوئر سيڪنڊري اسڪول وسڻ</h1>
    <p>SEMIS ID: 416040489 | ضلعو نوشهرو فيروز</p>
</header>

<nav>
    <a href="#home">هوم</a>
    <a href="#gallery">تصويرون</a>
    <a href="#result">رزلٽ</a>
    <a href="#contact">رابطو</a>
</nav>

<div class="container">
    
    <section id="gallery" class="card">
        <h2 style="color: var(--primary);">اسڪول جون تصويرون</h2>
        <div class="gallery">
            <img src="school1.jpg" alt="اسڪول جي بلڊنگ">
            <img src="staff.jpg" alt="اسڪول جو اسٽاف">
            <img src="students.jpg" alt="شاگرد">
        </div>
    </section>

    <section id="result" class="card">
        <h2 style="color: var(--primary);">آن لائن رزلٽ 2026</h2>
        <p>پنھنجو رول نمبر لکو:</p>
        <input type="text" id="rollNo" placeholder="مثال: 101">
        <button onclick="checkResult()">رزلٽ چيڪ ڪريو</button>
        <div id="resultDisplay" style="margin-top: 20px; font-weight: bold; font-size: 1.2em;"></div>
    </section>

    <section id="contact" class="card">
        <h2 style="color: var(--primary);">رابطو ۽ لوڪيشن</h2>
        <p>ايميل: gbelswassan@gmail.com</p>
        <a href="https://wa.me/923013875347" class="btn btn-wa">واٽس اپ تي رابطو ڪريو</a>
        <br><br>
        <iframe src="https://maps.google.com/?cid=10159834540914769955&g_mp=CiVnb29nbGUubWFwcy5wbGFjZXMudjEuUGxhY2VzLkdldFBsYWNl" width="100%" height="250" style="border:0; border-radius:10px;" allowfullscreen="" loading="lazy"></iframe>
        <a href="https://maps.app.goo.gl/uX8D1yA8V9j5Y2e2A6" target="_blank" class="btn btn-map">گوگل ميپ تي رستو ڏسو</a>
    </section>

</div>

<footer>
    <p>© 2026 GBELS وسڻ | سڀ حق محفوظ آهن</p>
    <p>ڊولپر: <a href="https://github.com/gbelswassan-cyber" style="color: var(--secondary);">gbelswassan-cyber</a></p>
</footer>

<script>
    function checkResult() {
        var roll = document.getElementById('rollNo').value;
        var display = document.getElementById('resultDisplay');
        
        // رزلٽ رڪارڊ
        var data = {
            "101": "نالو: محمد علي وسڻ | نمبر: 750 (A+)",
            "102": "نالو: احمد رضا | نمبر: 720 (A)",
            "103": "نالو: سائره ٻانو | نمبر: 710 (A)"
        };

        if(data[roll]) {
            display.style.color = "green";
            display.innerHTML = "✅ " + data[roll];
        } else {
            display.style.color = "red";
            display.innerHTML = "❌ معاف ڪجو، هي رول نمبر موجود ناهي.";
        }
    }
</script>

</body>
</html>

<div style="text-align: center; margin: 20px;">
    <a href="هتي_پنهنجي_فارم_جي_لنڪ_پيسٽ_ڪريو" target="_blank" 
       style="background-color: #d32f2f; color: white; padding: 15px 30px; text-decoration: none; border-radius: 30px; font-weight: bold; display: inline-block;">
        آن لائن داخلا فارم ڀريو 📝
    </a>
</div>
