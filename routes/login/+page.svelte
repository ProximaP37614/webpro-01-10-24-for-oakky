<script>
  import NavBar from '../component/NavBar.svelte'; // Adjust path based on location
</script>

<NavBar />

<div class="mx-20 sm:mx-28 md:mx-40 lg:mx-60 xl:mx-[34rem] mt-10 space-y-10">
  <div class="flex justify-center items-center">
    <p class="font-bold text-2xl sm:text-3xl md:text-4xl underline">เข้าสู่ระบบ</p>
  </div>

  <div class="space-y-6">
    <input
      type="text"
      placeholder="อีเมล / ชื่อผู้ใช้งาน"
      class="border-2 border-[#9F9F9F] rounded-lg w-full py-3 sm:py-4 md:py-5 p-4 sm:p-5 md:p-6 text-gray-500 text-left focus:outline-none focus:ring-2 focus:ring-gray-300"
    />
    <input
      type="text"
      placeholder="รหัสผ่าน"
      class="border-2 border-[#9F9F9F] rounded-lg w-full py-3 sm:py-4 md:py-5 p-4 sm:p-5 md:p-6 text-gray-500 text-left focus:outline-none focus:ring-2 focus:ring-gray-300"
    />
  </div>

  <button
    class="bg-[#102C57] text-white rounded-lg w-full py-3 sm:py-4 md:py-5 p-4 sm:p-5 md:p-6 focus:outline-none focus:ring-2 focus:ring-gray-300"
  >
    เข้าสู่ระบบ
  </button>
</div>

