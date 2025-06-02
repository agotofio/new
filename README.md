<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Free Fire Магазин</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      padding: 20px;
      background: #f5f5f5;
    }

    .product {
      background: white;
      border-radius: 10px;
      padding: 15px;
      margin-bottom: 30px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    .product img {
      max-width: 100%;
      height: auto;
      display: block;
      margin-bottom: 10px;
    }

    button {
      padding: 10px 20px;
      margin-top: 10px;
      cursor: pointer;
    }

    .modal {
      display: none;
      background: white;
      padding: 15px;
      border: 2px solid #ccc;
      border-radius: 10px;
      margin-top: 10px;
    }

    .modal input, .modal select {
      margin: 5px 5px 5px 0;
      padding: 5px;
    }
  </style>
</head>
<body>

  <!-- Алмазы -->
  <div class="product">
    <img src="https://cdn1.codashop.com/S/content/common/images/categories/diamond.png" alt="Алмазы">
    <h2>Алмазы</h2>
    <p>Пополнение от 100 до 5000 алмазов. Быстрая доставка.</p>
    <button onclick="toggleModal('diamondsModal')">Купить</button>
    <div id="diamondsModal" class="modal">
      <h3>Оформление заказа - Алмазы</h3>
      <label>Выберите способ оплаты:
        <select>
          <option>Крипта</option>
          <option>Карта</option>
          <option>Приват24</option>
        </select>
      </label>
      <input type="text" placeholder="0000 0000 0000 0000" />
      ID аккаунта Free Fire:
      <input type="text" placeholder="123456789" />
      <br>
      <button onclick="toggleModal('diamondsModal')">Отмена</button>
      <button>Отправить</button>
    </div>
  </div>

  <!-- Ваучеры -->
  <div class="product">
    <img src="https://cdn1.codashop.com/S/content/common/images/categories/voucher.png" alt="Ваучеры">
    <h2>Ваучеры</h2>
    <p>Скидки на элитный пропуск, эксклюзивные предметы.</p>
    <button onclick="toggleModal('voucherModal')">Купить</button>
    <div id="voucherModal" class="modal">
      <h3>Оформление заказа - Ваучеры</h3>
      <label>Выберите способ оплаты:
        <select>
          <option>Крипта</option>
          <option>Карта</option>
          <option>Приват24</option>
        </select>
      </label>
      <input type="text" placeholder="0000 0000 0000 0000" />
      ID аккаунта Free Fire:
      <input type="text" placeholder="123456789" />
      <br>
      <button onclick="toggleModal('voucherModal')">Отмена</button>
      <button>Отправить</button>
    </div>
  </div>

  <!-- Прокачка -->
  <div class="product">
    <img src="https://i.imgur.com/gh3aFYl.png" alt="Прокачка">
    <h2>Прокачка</h2>
    <p>Помощь с ранговыми играми и прокачкой персонажей.</p>
    <button onclick="toggleModal('boostModal')">Купить</button>
    <div id="boostModal" class="modal">
      <h3>Оформление заказа - Прокачка</h3>
      <label>Выберите способ оплаты:
        <select>
          <option>Крипта</option>
          <option>Карта</option>
          <option>Приват24</option>
        </select>
      </label>
      <input type="text" placeholder="0000 0000 0000 0000" />
      ID аккаунта Free Fire:
      <input type="text" placeholder="123456789" />
      <br>
      <button onclick="toggleModal('boostModal')">Отмена</button>
      <button>Отправить</button>
    </div>
  </div>

  <script>
    function toggleModal(id) {
      const modal = document.getElementById(id);
      modal.style.display = (modal.style.display === 'block') ? 'none' : 'block';
    }
  </script>

</body>
</html>
