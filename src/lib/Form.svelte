<script>
  import Button from './Button.svelte';
  import Comparison from '../assets/form.png';
</script>

<form action="" class="form">
  <p class="form-header">
    サカイ・アート
    <span class="form-header-smaller">など</span>
    人気業者<span class="form-header-smaller">を</span>徹底比較！
  </p>
  <div class="form-body">
    <div class="form-item">
      <p class="form-label">現在の郵便局</p>
      <input class="form-input" type="text" placeholder="例）1500001">
    </div>
    <div class="form-item">
      <p class="form-label">引越し先</p>
      <select name="" class="form-select">
        <option value="1">北海道</option>
        <option value="2">秋田県</option>
        <option value="3">千葉県</option>
        <option value="6" selected>東京都</option>
        <option value="4">愛知県</option>
        <option value="5">京都府</option>
        <option value="7">福岡県</option>
      </select>
    </div>
    <div class="form-item">
      <p class="form-label">引越しタイプ</p>
      <div class="form-radio">
        <label for="move-type-1" class="form-radio-item"><input id="move-type-1" type="radio" name="move-type" checked ><span>単身</span></label>
        <label for="move-type-2" class="form-radio-item"><input id="move-type-2" type="radio" name="move-type"><span>家族</span></label>
      </div>
    </div>
    <Button />
    <p class="form-lead">カンタン60秒！最安値の業者がすぐわかる！</p>
    <img src={Comparison} alt="最大10社が比較可能！" class="form-image" />
  </div>
</form>


<style>
  .form {
    border: 1px solid #00a022;
    border-top: 4px solid #00a022;
  }

  .form-header {
    padding: 6px 0;
    background-color: #e4f3cc;
    color: #00a022;
    font-size: 16px;
    font-weight: bold;
    text-align: center;
  }

  .form-header-smaller {
    font-size: 13px;
  }

  .form-body {
    padding: 12px;
    background-color: #fff;
    font-size: 14px;
  }

  .form-image {
    width: 100%;
    margin: auto;
  }

  .form-lead {
    margin: 16px 0;
    font-size: 14px;
    font-weight: bold;
  }

  .form-item {
    display: grid;
    grid-template-columns: 130px 1fr;
    align-items: center;
    margin-bottom: 4px;
  }

  .form-label {
    text-align: left;
  }

  .form-input,
  .form-select {
    box-sizing: border-box;
    border: 2px solid #ddd;
    border-radius: 4px;
    line-height: 1.6;
  }

  .form-input {
    padding: 6px 8px;
    font-size: 16px;
  }

  .form-select {
    padding: 8px;
    font-size: 14px;
  }

  .form-radio {
    display: grid;
    grid-template-columns: 1fr 1fr;
    box-sizing: border-box;
    border: 2px solid #ddd;
    border-radius: 4px;
  }

  .form-radio > *:first-child {
    border-right: 2px solid #ddd;
  }

  .form-radio-item {
    padding: 6px;
    box-sizing: border-box;
  }
</style>
