<script setup>
</script>

<template>
  <main>
    <div class="">
      <input type="text" list="pharmacies-retail" placeholder="Select Pharmacy ..">

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
              <td>Health Care Pharm <span>Amir</span></td>
              <td>420</td>
            </tr>
            <tr>
              <td>Healit Ointment</td>
              <td>Health Care Pharm <span>Amir</span></td>
              <td>420</td>
            </tr>
            <tr>
              <td>Healit Ointment</td>
              <td>Health Care Pharm <span>Amir</span></td>
              <td>420</td>
            </tr>
          </tbody>
        </table>
      </div>
      <div class="add-icon">
        +
      </div>
    </div>
  </main>
</template>

<style scoped>
  input{
    border: none;
    padding: .4rem 1rem;
    background-color: lightgoldenrodyellow;
    border-radius: 30px;
    box-shadow: 0 2px 4px -4px black;
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

