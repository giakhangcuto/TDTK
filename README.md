# TDTK
<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <title>Màn hình 1: Trang chủ - TrọSV</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
  <style>
    body { background-color: #0f172a; display: flex; justify-content: center; align-items: center; min-height: 100vh; font-family: 'Segoe UI', sans-serif; }
    .phone-frame { width: 375px; height: 780px; background: #ffffff; border-radius: 42px; border: 10px solid #1e293b; box-shadow: 0 25px 50px -12px rgba(0,0,0,0.6); overflow: hidden; display: flex; flex-direction: column; position: relative; }
    .notch { width: 150px; height: 24px; background: #1e293b; border-bottom-left-radius: 16px; border-bottom-right-radius: 16px; margin: 0 auto; }
  </style>
</head>
<body>

  <div class="phone-frame">
    <!-- Tai thỏ & Thanh trạng thái -->
    <div class="bg-white pt-1 pb-2 px-6 flex justify-between items-center text-xs font-semibold text-gray-800">
      <span>9:41</span>
      <div class="notch -mt-2"></div>
      <div class="flex gap-1.5 items-center">
        <i class="fa-solid fa-signal"></i>
        <i class="fa-solid fa-wifi"></i>
        <i class="fa-solid fa-battery-full text-sm"></i>
      </div>
    </div>

    <!-- KHU VỰC 1: Header Logo & Icon -->
    <div class="px-4 py-2 flex justify-between items-center bg-white">
      <div class="flex items-center gap-2">
        <div class="w-9 h-9 rounded-xl bg-emerald-600 flex items-center justify-center text-white shadow-sm">
          <i class="fa-solid fa-graduation-cap text-lg"></i>
        </div>
        <span class="text-2xl font-extrabold tracking-tight text-emerald-700">Trọ<span class="text-sky-600">SV</span></span>
      </div>
      <div class="flex gap-3 text-gray-600 text-lg">
        <button class="relative hover:text-emerald-600">
          <i class="fa-regular fa-bell"></i>
          <span class="absolute -top-1 -right-1 w-2.5 h-2.5 bg-red-500 rounded-full"></span>
        </button>
        <button class="hover:text-red-500">
          <i class="fa-regular fa-heart"></i>
        </button>
      </div>
    </div>

    <!-- KHU VỰC 2: Thanh tìm kiếm & Bộ lọc -->
    <div class="px-4 py-2 bg-white">
      <div class="bg-gray-100 rounded-full px-4 py-2.5 flex items-center gap-2.5 border border-gray-200">
        <i class="fa-solid fa-magnifying-glass text-gray-400"></i>
        <input type="text" placeholder="Tìm kiếm trọ gần trường ĐH..." class="bg-transparent text-sm w-full outline-none text-gray-700" />
      </div>

      <!-- 4 Nút bộ lọc nhanh -->
      <div class="grid grid-cols-4 gap-2 mt-3 text-center">
        <div class="bg-emerald-50 border border-emerald-300 rounded-xl p-2 cursor-pointer shadow-sm">
          <div class="text-emerald-600 text-base"><i class="fa-solid fa-circle-check"></i></div>
          <div class="text-[11px] font-bold text-emerald-800 mt-1">Đã kiểm chứng</div>
        </div>
        <div class="bg-amber-50 border border-amber-200 rounded-xl p-2 cursor-pointer">
          <div class="text-amber-500 text-base"><i class="fa-solid fa-sack-dollar"></i></div>
          <div class="text-[11px] font-semibold text-gray-700 mt-1">Giá rẻ</div>
        </div>
        <div class="bg-sky-50 border border-sky-200 rounded-xl p-2 cursor-pointer">
          <div class="text-sky-600 text-base"><i class="fa-solid fa-user-group"></i></div>
          <div class="text-[11px] font-semibold text-gray-700 mt-1">Ở ghép</div>
        </div>
        <div class="bg-purple-50 border border-purple-200 rounded-xl p-2 cursor-pointer">
          <div class="text-purple-600 text-base"><i class="fa-solid fa-school"></i></div>
          <div class="text-[11px] font-semibold text-gray-700 mt-1">Gần trường</div>
        </div>
      </div>
    </div>

    <!-- KHU VỰC 3: Banner Đặc quyền Đã Kiểm Định & AR/1x -->
    <div class="px-4 my-2">
      <div class="bg-gradient-to-r from-sky-600 to-emerald-500 rounded-2xl p-4 text-white shadow-md relative overflow-hidden">
        <span class="bg-white/20 text-[10px] font-bold uppercase px-2 py-0.5 rounded-full">Tính năng cốt lõi</span>
        <h2 class="text-base font-extrabold mt-1 leading-snug">ĐẶC QUYỀN ĐÃ KIỂM ĐỊNH</h2>
        <p class="text-xs text-white/95 mt-0.5">Phòng trọ đã được Nhà trường/CLB khảo sát thực tế • Tích hợp <b>AR đo phòng</b> & <b>Video Call khóa 1x</b></p>
      </div>
    </div>

    <!-- KHU VỰC 4: Danh sách tin đăng -->
    <div class="px-4 flex-1 overflow-y-auto space-y-3 pb-4">
      <div class="flex justify-between items-center">
        <h3 class="font-bold text-gray-800 text-sm">Danh sách tin đăng uy tín</h3>
        <span class="text-xs text-emerald-600 font-semibold cursor-pointer">Xem tất cả</span>
      </div>

      <!-- Thẻ phòng 1 -->
      <div class="bg-white border border-gray-200 rounded-2xl p-2.5 flex gap-3 shadow-sm hover:border-emerald-400 cursor-pointer">
        <img src="https://images.unsplash.com/photo-1522708323590-d24dbb6b0267?w=300&q=80" alt="Phòng trọ Quận 10" class="w-24 h-24 rounded-xl object-cover" />
        <div class="flex-1 flex flex-col justify-between">
          <div>
            <div class="flex justify-between items-start">
              <h4 class="font-bold text-gray-800 text-sm">Phòng trọ Quận 10</h4>
              <span class="bg-emerald-100 text-emerald-700 text-[10px] font-bold px-1.5 py-0.5 rounded">AR + 1x</span>
            </div>
            <p class="text-emerald-600 font-extrabold text-sm mt-0.5">3.5tr/tháng <span class="text-gray-400 font-normal text-xs">• 14.4m²</span></p>
          </div>
          <div class="space-y-0.5">
            <p class="text-[11px] text-emerald-700 font-semibold flex items-center gap-1">
              <i class="fa-solid fa-circle-check"></i> Đã kiểm chứng bởi CLB/Trường
            </p>
            <p class="text-[11px] text-gray-500 flex items-center gap-1">
              <i class="fa-solid fa-location-dot text-red-500"></i> 3.2km đến trường
            </p>
          </div>
        </div>
      </div>

      <!-- Thẻ phòng 2 -->
      <div class="bg-white border border-gray-200 rounded-2xl p-2.5 flex gap-3 shadow-sm hover:border-emerald-400 cursor-pointer">
        <img src="https://images.unsplash.com/photo-1598928506311-c55ded91a20c?w=300&q=80" alt="Phòng trọ Bình Chánh" class="w-24 h-24 rounded-xl object-cover" />
        <div class="flex-1 flex flex-col justify-between">
          <div>
            <div class="flex justify-between items-start">
              <h4 class="font-bold text-gray-800 text-sm">Phòng trọ ghép Bình Chánh</h4>
              <span class="bg-sky-100 text-sky-700 text-[10px] font-bold px-1.5 py-0.5 rounded">Ở ghép</span>
            </div>
            <p class="text-emerald-600 font-extrabold text-sm mt-0.5">1.8tr/tháng <span class="text-gray-400 font-normal text-xs">• 18m²</span></p>
          </div>
          <div class="space-y-0.5">
            <p class="text-[11px] text-emerald-700 font-semibold flex items-center gap-1">
              <i class="fa-solid fa-circle-check"></i> Đã kiểm chứng bởi CLB/Trường
            </p>
            <p class="text-[11px] text-gray-500 flex items-center gap-1">
              <i class="fa-solid fa-location-dot text-red-500"></i> Gần khu ĐH Nguyễn Văn Linh
            </p>
          </div>
        </div>
      </div>
    </div>

    <!-- KHU VỰC 5: Thanh điều hướng dưới cùng (Bottom Nav) -->
    <div class="bg-white border-t border-gray-200 px-4 py-2 flex justify-between items-center text-[11px] text-gray-500">
      <div class="flex flex-col items-center text-emerald-600 font-bold cursor-pointer">
        <i class="fa-solid fa-house text-base"></i>
        <span class="mt-0.5">Trang chủ</span>
      </div>
      <div class="flex flex-col items-center hover:text-emerald-600 cursor-pointer">
        <i class="fa-solid fa-map-location-dot text-base"></i>
        <span class="mt-0.5">Bản đồ</span>
      </div>
      <div class="flex flex-col items-center hover:text-emerald-600 cursor-pointer">
        <i class="fa-solid fa-square-plus text-base"></i>
        <span class="mt-0.5">Đăng tin</span>
      </div>
      <div class="flex flex-col items-center hover:text-emerald-600 cursor-pointer">
        <i class="fa-regular fa-comment-dots text-base"></i>
        <span class="mt-0.5">Tin nhắn</span>
      </div>
      <div class="flex flex-col items-center hover:text-emerald-600 cursor-pointer">
        <i class="fa-regular fa-user text-base"></i>
        <span class="mt-0.5">Cá nhân</span>
      </div>
    </div>
  </div>

</body>
</html>
