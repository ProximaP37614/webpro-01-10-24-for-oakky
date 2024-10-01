<script>
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

  <div class="mx-20 sm:mx-28 md:mx-40 lg:mx-60 xl:mx-[34rem] mt-10 space-y-10">
    <div class="flex justify-center items-center">
      <p class="font-bold text-2xl sm:text-3xl md:text-4xl underline">ลงทะเบียนเข้าสู่ระบบ</p>
    </div>
  
    <div class="space-y-6">
        <div class="flex items-center border-2 border-[#9F9F9F] rounded-lg w-full py-3 sm:py-4 md:py-5 p-3 sm:p-3 md:p-3 text-gray-500 text-left focus:outline-none focus:ring-2 focus:ring-gray-300">
        <input
            type="text"
            class="flex-grow px-2 py-1 focus:outline-none"
            placeholder="อีเมล / ชื่อผู้ใช้งาน"
        />
        <button
            class="ml-2 bg-gray-300 text-gray-500 py-1 px-4 rounded-lg hover:bg-gray-400 focus:outline-none"
        >
            ยืนยัน
        </button>
        </div>
      <input
        type="text"
        placeholder="รหัสผ่าน"
        class="border-2 border-[#9F9F9F] rounded-lg w-full py-3 sm:py-4 md:py-5 p-4 sm:p-5 md:p-6 text-gray-500 text-left focus:outline-none focus:ring-2 focus:ring-gray-300"
      />
      <input
        type="text"
        placeholder="ยืนยันรหัสผ่าน"
        class="border-2 border-[#9F9F9F] rounded-lg w-full py-3 sm:py-4 md:py-5 p-4 sm:p-5 md:p-6 text-gray-500 text-left focus:outline-none focus:ring-2 focus:ring-gray-300"
      />
    </div>
  
    <hr class="h-px my-8 bg-[#9F9F9F] border-0 ">

    <div class="space-y-6">
        <p class="text-[#590606] underline font-medium">กรุณากรอกข้อมูลให้ครบถ้วน</p>
      <input
        type="text"
        placeholder="ชื่อจริง"
        class="border-2 border-[#9F9F9F] rounded-lg w-full py-3 sm:py-4 md:py-5 p-4 sm:p-5 md:p-6 text-gray-500 text-left focus:outline-none focus:ring-2 focus:ring-gray-300"
      />
      <input
        type="text"
        placeholder="นามสกุล"
        class="border-2 border-[#9F9F9F] rounded-lg w-full py-3 sm:py-4 md:py-5 p-4 sm:p-5 md:p-6 text-gray-500 text-left focus:outline-none focus:ring-2 focus:ring-gray-300"
      />
      <input
        type="text"
        placeholder="เบอร์โทรศัพท์"
        class="border-2 border-[#9F9F9F] rounded-lg w-full py-3 sm:py-4 md:py-5 p-4 sm:p-5 md:p-6 text-gray-500 text-left focus:outline-none focus:ring-2 focus:ring-gray-300"
      />
      <input
        type="text"
        placeholder="เลขบัตรประจำตัวประชาชน"
        class="border-2 border-[#9F9F9F] rounded-lg w-full py-3 sm:py-4 md:py-5 p-4 sm:p-5 md:p-6 text-gray-500 text-left focus:outline-none focus:ring-2 focus:ring-gray-300"
      />
      
        <div class="flex items-center mb-4">
            <input type="checkbox" class="accent-[#D9D9D9] w-6 h-6">
            <label for="default-checkbox" class="ms-2 text-sm font-medium text-gray-900 dark:text-gray-300">[จำเป็น] ข้าพเจ้าได้ตรวจสอบ เงื่อนไขการใช้บริการของ........ แล้ว และตกลงยอมรับ</label>
        </div>
        <div class="flex items-center">
            <input type="checkbox" class="accent-[#D9D9D9] w-6 h-6">
            <label for="checked-checkbox" class="ms-2 text-sm font-medium text-gray-900 dark:text-gray-300">[จำเป็น] ข้าพเจ้าได้ตรวจสอบ นโยบายการจัดการข้อมูลส่วนบุคล แล้ว และตกลงยอมรับ</label>
        </div>
        <button
        class="bg-[#102C57] text-white rounded-lg w-full py-3 sm:py-4 md:py-5 p-4 sm:p-5 md:p-6 focus:outline-none focus:ring-2 focus:ring-gray-300"
      >
        เข้าสู่ระบบ
      </button>
    </div>
    
  </div>
  
  