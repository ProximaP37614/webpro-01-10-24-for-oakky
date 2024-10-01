<script>
    let email = '';
    let firstName = '';
    let lastName = '';
    let cardNumber = '';
    let expiryDate = '';
    let cvc = '';
    let isMenuOpen = false;

  function toggleMenu() {
    isMenuOpen = !isMenuOpen;
  }
  </script>

<header class="bg-[#102C57]">
    <nav class="flex justify-between items-center h-24 w-[92%] mx-auto font-body">
      <div>
        <a class="text-white font-bold text-xl">OURTRIN</a>
      </div>
  
      <div class="flex">
        <div class={`md:static absolute bg-[#102C57] md:min-h-fit min-h-[30vh] left-0 ${isMenuOpen ? 'top-[9%]' : 'top-[-100%]'} md:w-auto w-full flex items-center px-5`}>
          <ul class="flex md:flex-row flex-col md:items-center md:gap-[4vw] gap-8">
            <li>
              <a class="text-white hover:text-gray-500" href="main">ค้นหาเที่ยวโดยสาร</a>
            </li>
            <li>
              <a class="text-white hover:text-gray-500" href="main">รายการตั๋วโดยสาร</a>
            </li>
            <li>
              <a class="text-white hover:text-gray-500" href="main">ลงทะเบียน</a>
            </li>
          </ul>
        </div>
  
        <img
          on:click={toggleMenu}
          name={isMenuOpen ? 'close' : 'menu'}
          class="text-3xl text-white cursor-pointer md:hidden size-16"
          src="https://static.thenounproject.com/png/4238597-200.png"
        >
      </div>
    </nav>
  </header>

  <div class="flex flex-col md:flex-row md:justify-between items-center p-8">
    <!-- Payment Form Section -->
    <div class="w-full md:w-1/2">
      <div class="mb-4">
        <label class="block mb-2 text-[#102C57] font-extrabold text-xl">เลือกวิธีการชำระเงิน</label>
        <div class="border border-[#9F9F9F] rounded-lg p-2 flex justify-between">
          <select class="w-full focus:outline-none text-[#9F9F9F]">
            <option>วิธีการชำระเงิน</option>
            <option>วิธีการชำระเงิน</option>
            <option>วิธีการชำระเงิน</option>
          </select>
        </div>
      </div>
  
      <div class="border-t border-black my-4"></div>
  
      <div class="mb-4">
        <label class="block mb-2 text-[#102C57] font-extrabold text-xl">ข้อมูลส่วนบุคคล</label>
        <div class="border-2 border-dashed border-[#9747FF] rounded-lg p-4">
          <!-- Email -->
          <div class="mb-3">
            <input
              type="text"
              placeholder="อีเมล"
              class="w-full p-2 border border-[#9F9F9F] rounded-lg focus:outline-none"
              bind:value={email}
            />
          </div>
  
          <!-- Name -->
          <div class="grid grid-cols-2 gap-3 mb-3">
            <input
              type="text"
              placeholder="ชื่อจริง"
              class="p-2 border border-[#9F9F9F] rounded-lg focus:outline-none"
              bind:value={firstName}
            />
            <input
              type="text"
              placeholder="นามสกุล"
              class="p-2 border border-[#9F9F9F] rounded-lg focus:outline-none"
              bind:value={lastName}
            />
          </div>
  
          <!-- Card Number -->
          <div class="mb-3">
            <input
              type="text"
              placeholder="หมายเลขบัตร"
              class="w-full p-2 border border-[#9F9F9F] rounded-lg focus:outline-none"
              bind:value={cardNumber}
            />
          </div>
  
          <!-- Expiry Date and CVC -->
          <div class="grid grid-cols-2 gap-3 mb-3">
            <input
              type="text"
              placeholder="วันหมดอายุ"
              class="p-2 border border-[#9F9F9F] rounded-lg focus:outline-none"
              bind:value={expiryDate}
            />
            <input
              type="text"
              placeholder="CVC / หมายเลขหลังบัตร"
              class="p-2 border border-[#9F9F9F] rounded-lg focus:outline-none"
              bind:value={cvc}
            />
          </div>
  
          <!-- Payment Button -->
          <div class="text-right">
            <button class="bg-[#102C57] text-white py-2 px-4 rounded-lg">
              ชำระเงิน
            </button>
          </div>
        </div>
      </div>
    </div>
  
    <!-- Image and Text Section -->
    <div class="w-full md:w-1/2 mt-8 md:mt-0 flex flex-col items-center">
        <div class="flex flex-col justify-center items-center mx-8 space-y-8">
            <h2 class="text-[#102C57] text-3xl font-black mb-4 underline">คุณเตรียมตัวเดินทาง เราจะพาคุณไปถึงจุดหมาย</h2>
            <img
                src="https://cdn-icons-png.flaticon.com/512/235/235861.png"
                alt="Map Icon"
                class="w-40 h-40"
            />
        </div>
    </div>
  </div>
  