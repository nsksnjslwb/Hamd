<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>موقع الرياضة</title>
  <style>
    body {
      font-family: 'Segoe UI', Arial, sans-serif;
      background: linear-gradient(135deg, #e0f7fa, #b2ebf2);
      text-align: center;
      padding: 20px;
      margin: 0;
    }

    h1 {
      color: #00796b;
      font-size: 32px;
      margin-bottom: 20px;
    }

    .sport-img {
      width: 90%;
      max-width: 350px;
      border-radius: 20px;
      margin: 20px auto;
      display: block;
      box-shadow: 0 6px 12px rgba(0,0,0,0.2);
    }

    .card {
      background: #ffffffcc;
      margin: 15px auto;
      padding: 20px;
      width: 95%;
      max-width: 320px;
      border-radius: 15px;
      box-shadow: 0 8px 16px rgba(0,0,0,0.15);
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 12px 24px rgba(0,0,0,0.25);
    }

    h2 {
      color: #004d40;
      font-size: 22px;
      margin-bottom: 10px;
    }

    .card p {
      font-size: 17px;
      line-height: 1.5;
      color: #333;
    }

    .start-btn {
      background-color: #00796b;
      color: white;
      padding: 15px 30px;
      font-size: 18px;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      margin: 30px auto;
      transition: background-color 0.3s, transform 0.2s;
      display: block;
    }

    .start-btn:hover {
      background-color: #004d40;
      transform: scale(1.05);
    }

    /* قسم النصائح مخفي */
    #tips-section {
      display: none;
      margin-top: 30px;
    }

    .tip-card {
      background: #ffffffcc;
      margin: 15px auto;
      padding: 20px;
      width: 95%;
      max-width: 320px;
      border-radius: 15px;
      box-shadow: 0 8px 16px rgba(0,0,0,0.15);
    }

    .tip-card img {
      width: 100%;
      max-width: 280px;
      border-radius: 15px;
      margin-bottom: 15px;
      display: block;
    }

    .back-btn {
      background-color: #e65100;
      color: white;
      padding: 12px 25px;
      font-size: 18px;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      margin-top: 20px;
      transition: background-color 0.3s, transform 0.2s;
      display: block;
    }

    .back-btn:hover {
      background-color: #bf360c;
      transform: scale(1.05);
    }
  </style>
</head>
<body>

  <h1>🏋️‍♂️ موقع الرياضة</h1>
  <img src="https://www.w3schools.com/html/pic_trulli.jpg" class="sport-img">
  <p>ابدأ رحلتك نحو جسم صحي</p>

  <div class="card">
    <h2>تمارين يومية</h2>
    <p>10 دقائق حركة كل يوم تصنع فرق كبير 💥</p>
  </div>

  <div class="card">
    <h2>تغذية صحية</h2>
    <p>اكل متوازن مليء بالخضار والفواكه يمنحك طاقة 🌱</p>
  </div>

  <div class="card">
    <h2>نصائح عامة</h2>
    <p>نام زين، اشرب مي، وداوم 👌</p>
  </div>

  <button class="start-btn" onclick="showTips()">ابدأ التمارين</button>

  <!-- قسم النصائح -->
  <div id="tips-section">
    <h1>💡 نصائح الرياضة</h1>

    <div class="tip-card">
      <img src="https://www.w3schools.com/html/img_chania.jpg">
      <h2>التمارين اليومية</h2>
      <p>حاول تتحرك 30 دقيقة يوميًا للحفاظ على صحتك 💪</p>
    </div>

    <div class="tip-card">
      <img src="https://www.w3schools.com/html/img_girl.jpg">
      <h2>التغذية السليمة</h2>
      <p>اكل متوازن مليء بالخضار والفواكه يمنحك طاقة 🌱</p>
    </div>

    <div class="tip-card">
      <img src="https://www.w3schools.com/html/img_lights.jpg">
      <h2>الراحة والنوم</h2>
      <p>احرص على نوم كافي للحفاظ على قوة جسمك 🛌</p>
    </div>

    <button class="back-btn" onclick="hideTips()">عودة للصفحة الرئيسية</button>
  </div>

  <script>
    function showTips() {
      document.getElementById('tips-section').style.display = 'block';
      window.scrollTo(0,0);
    }

    function hideTips() {
      document.getElementById('tips-section').style.display = 'none';
      window.scrollTo(0,0);
    }
  </script>

</body>
</html>
