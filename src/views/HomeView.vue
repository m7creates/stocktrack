<script setup>

</script>

<template>
  <main>
    <div class="select-pharmacy">
      Select Pharmacy |
      <input type="text" list="pharmacies-retail" placeholder="Click and type ..">

      <datalist id="pharmacies-retail">
        <option value="Higher Life Pharm" />
        <option value="Parents Pharm" />
        <option value="Joso Pharm" />
      </datalist>
    </div>
    
    <div class="">
      <div class="">
        <input type="search" placeholder="Search ...">
        <table>
          <thead>
            <tr>
              <th>Drug</th>
              <th>Supplier</th>
              <th>Rate@</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Healit Ointment</td>
              <td>Health Care Pharm <span>(Amir)</span></td>
              <td>7,000</td>
            </tr>
            <tr>
              <td>Aquasoft Lotion</td>
              <td>Abacus Pharma <span>(Okello)</span></td>
              <td>16,500</td>
            </tr>
            <tr>
              <td>Kidibar Soap & Lotion</td>
              <td>Sky Phamacy <span>(Fatuma)</span></td>
              <td>17,500</td>
            </tr>
          </tbody>
        </table>
      </div>

      <!-- <div class="">
        <form @submit.prevent="submitForm" id="add-drug-form">
          <div>
            <label for="drug">Drug:</label>
            <input type="text" id="drug" v-model="formData.drug" required>
          </div>
          <div>
            <label for="brand_name">Brand Name:</label>
            <input type="text" id="brand_name" v-model="formData.brand_name" required>
          </div>
          <div>
            <label for="current_count">Current Count:</label>
            <input type="number" id="current_count" v-model="formData.current_count" required>
          </div>
          <div>
            <label for="drugs_contained">Drugs Contained:</label>
            <input type="text" id="drugs_contained" v-model="formData.drugs_contained" required>
          </div>
          <div>
            <label for="expiry_date">Expiry Date:</label>
            <input type="date" id="expiry_date" v-model="formData.expiry_date" required>
          </div>
          <div>
            <label for="form">Form:</label>
            <input type="text" id="form" v-model="formData.form" required>
          </div>
          <div>
            <label for="manufacturer">Manufacturer:</label>
            <input type="text" id="manufacturer" v-model="formData.manufacturer" required>
          </div>
          <div>
            <label for="supplier">Supplier:</label>
            <input type="text" id="supplier" v-model="formData.supplier" required>
          </div>
          <div>
            <label for="rate">Rate@:</label>
            <input type="number" id="rate" v-model="formData.rate" required>
          </div>
            <button type="submit">Add</button>
        </form>
      </div> -->

      <div class="add-icon">
        +
      </div>
    </div>
  </main>
</template>

<style scoped>
  input {
    border: 1px solid #ccc;
    padding: 0.6rem 1rem;
    background-color: #fff;
    border-radius: 4px;
    box-shadow: 0 0 3px rgba(24, 24, 24, 0.1);
    font-size: 1rem;
    transition: all 0.3s ease;
  }

  .select-pharmacy{
    margin: 1rem 0 .4rem;
    border: 1px solid #ccc;
    padding: 0.6rem 1rem; border-radius: 4px;
  }

  .select-pharmacy input {
    all: unset;
    border: none;
    padding: 0;
    font-size: 1.2rem;
  } 
  /* .select-pharmacy input{all: unset;} */

  input:focus {
    border-color: var(--primary-color);
    box-shadow: 0 0 5px rgba(0, 123, 255, 0.5);
    outline: none;
  }

  .add-icon{
    background-color: var(--primary-color);
    color: white;
    border-radius: 50%;
    width: 2.4rem;
    height: 2.4rem;
    display: flex;
    justify-content: center;
    align-items: center;

    cursor: pointer;
    font-size: 2rem;
  }

  table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 1rem;
    background-color: #f9f9f9;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    overflow: hidden;
  }

  th, td {
    padding: 0.8rem 1rem;
    text-align: left;
    border-bottom: 1px solid #ddd;
  }

  th {
    background-color: #333;
    color: white;
    font-weight: bold;
    text-transform: uppercase;
  }

  tr:hover {
    background-color: #f1f1f1;
  }

  td {
    color: #555;
  }

  tbody tr:last-child td {
    border-bottom: none;
  }
</style>

