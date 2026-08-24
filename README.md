# 2011jarvisdodoo-ux.github.io
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>JCF | Roblox Fighter Rankings</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      background: #f5f5f5;
      color: #111;
    }

    header {
      background: #111;
      color: white;
      height: 72px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 6%;
    }

    .logo {
      font-size: 34px;
      font-weight: 900;
      letter-spacing: -2px;
    }

    nav {
      display: flex;
      gap: 35px;
      font-weight: bold;
      font-size: 14px;
    }

    nav a {
      color: white;
      text-decoration: none;
    }

    .hero {
      background: white;
      padding: 70px 6% 45px;
      border-bottom: 1px solid #ddd;
    }

    .small-title {
      color: #d40000;
      font-size: 14px;
      font-weight: 800;
      letter-spacing: 2px;
      margin-bottom: 12px;
    }

    h1 {
      font-size: clamp(42px, 8vw, 90px);
      font-weight: 900;
      letter-spacing: -4px;
      line-height: .9;
    }

    .ranking {
      max-width: 1200px;
      margin: 0 auto;
      padding: 50px 6%;
    }

    .division {
      margin-bottom: 55px;
    }

    .division-title {
      border-bottom: 4px solid #111;
      padding-bottom: 12px;
      margin-bottom: 0;
      font-size: 24px;
      font-weight: 900;
    }

    .fighter {
      background: white;
      min-height: 150px;
      border-bottom: 1px solid #ddd;
      display: flex;
      align-items: center;
      position: relative;
      overflow: hidden;
      cursor: pointer;
      transition: .2s;
    }

    .fighter:hover {
      background: #eeeeee;
    }

    .rank {
      width: 80px;
      text-align: center;
      font-size: 24px;
      font-weight: 900;
      color: #999;
    }

    .fighter-info {
      flex: 1;
      padding: 25px;
      z-index: 2;
    }

    .status {
      color: #d40000;
      font-size: 12px;
      font-weight: 900;
      letter-spacing: 1px;
      margin-bottom: 7px;
    }

    .fighter-name {
      font-size: clamp(25px, 4vw, 43px);
      font-weight: 900;
      text-transform: uppercase;
    }

    .record {
      margin-top: 7px;
      color: #666;
      font-size: 14px;
    }

    .fighter-image {
      width: 190px;
      height: 150px;
      object-fit: contain;
      align-self: flex-end;
      margin-right: 40px;
    }

    .arrow {
      font-size: 28px;
      padding: 20px;
    }

    .details {
      display: none;
      background: #181818;
      color: white;
      padding: 25px 35px;
    }

    .details.open {
      display: block;
    }

    .stats {
      display: flex;
      gap: 35px;
      flex-wrap: wrap;
    }

    .stat strong {
      display: block;
      font-size: 22px;
    }

    .stat span {
      color: #aaa;
      font-size: 11px;
      text-transform: uppercase;
    }

    footer {
      background: #111;
      color: #aaa;
      text-align: center;
      padding: 35px;
      font-size: 13px;
    }

    @media (max-width: 700px) {
      header {
        padding: 0 20px;
      }

      nav {
        display: none;
      }

      .hero {
        padding: 50px 20px 35px;
      }

      .ranking {
        padding: 35px 15px;
      }

      .fighter {
        min-height: 120px;
      }

      .rank {
        width: 45px;
        font-size: 18px;
      }

      .fighter-info {
        padding: 15px 8px;
      }

      .fighter-image {
        width: 105px;
        height: 115px;
        margin-right: 5px;
      }

      .arrow {
        padding: 10px;
      }
    }
  </style>
</head>

<body>

<header>
  <div class="logo">JCF</div>

  <nav>
    <a href="#">HOME</a>
    <a href="#">EVENTS</a>
    <a href="#">RANKINGS</a>
    <a href="#">ATHLETES</a>
    <a href="#">NEWS</a>
  </nav>
</header>

<section class="hero">
  <div class="small-title">OFFICIAL RANKINGS</div>
  <h1>JCF ROBLOX<br>RANKINGS</h1>
</section>

<main class="ranking">

  <section class="division">
    <div class="division-title">HEAVYWEIGHT</div>

    <div class="fighter" onclick="toggleDetails(this)">
      <div class="rank">C</div>

      <div class="fighter-info">
        <div class="status">JCF CHAMPION</div>
        <div class="fighter-name">FIGHTER NAME</div>
        <div class="record">0-0-0</div>
      </div>

      <img class="fighter-image"
           src="https://placehold.co/300x300"
           alt="Roblox fighter">

      <div class="arrow">⌄</div>
    </div>

    <div class="details">
      <div class="stats">
        <div class="stat">
          <strong>0-0-0</strong>
          <span>Record</span>
        </div>

        <div class="stat">
          <strong>0</strong>
          <span>KO Wins</span>
        </div>

        <div class="stat">
          <strong>0</strong>
          <span>Sub Wins</span>
        </div>

        <div class="stat">
          <strong>0</strong>
          <span>Win Streak</span>
        </div>
      </div>
    </div>
  </section>

  <section class="division">
    <div class="division-title">LIGHTWEIGHT</div>

    <div class="fighter" onclick="toggleDetails(this)">
      <div class="rank">C</div>

      <div class="fighter-info">
        <div class="status">JCF CHAMPION</div>
        <div class="fighter-name">FIGHTER NAME</div>
        <div class="record">0-0-0</div>
      </div>

      <img class="fighter-image"
           src="https://placehold.co/300x300"
           alt="Roblox fighter">

      <div class="arrow">⌄</div>
    </div>

    <div class="details">
      <div class="stats">
        <div class="stat">
          <strong>0-0-0</strong>
          <span>Record</span>
        </div>

        <div class="stat">
          <strong>0</strong>
          <span>KO Wins</span>
        </div>

        <div class="stat">
          <strong>0</strong>
          <span>Sub Wins</span>
        </div>
      </div>
    </div>
  </section>

</main>

<footer>
  © 2026 JCF — Roblox Fighter Rankings
</footer>

<script>
function toggleDetails(fighter) {
  const details = fighter.nextElementSibling;
  details.classList.toggle("open");
}
</script>

</body>
</html>
