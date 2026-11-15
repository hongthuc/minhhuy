<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=5.0">
    <title>CÔNG TY TNHH MAI BẢO CHÂU - Showroom VLXD & Nội Thất Minh Huy | minhhuy.com</title>
    <meta name="description" content="Công Ty TNHH Mai Bảo Châu (minhhuy.com) - Showroom Minh Huy tại 199 Xô Viết Nghệ Tĩnh, Cẩm Lệ, Đà Nẵng. Chuyên Sơn, Thiết bị vệ sinh, Gạch men, Ngói lợp, Bồn nước, Bình nóng lạnh, Keo dán gạch chính hãng. ĐT: 0932.555.605">

    <!-- Thumbnail là ảnh Logo trang web khi gửi link chia sẻ qua Zalo / Facebook -->
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://minhhuy.com/">
    <meta property="og:title" content="CÔNG TY TNHH MAI BẢO CHÂU - Nội Thất & VLXD Minh Huy (minhhuy.com)">
    <meta property="og:description" content="Showroom Gạch Men, Thiết Bị Vệ Sinh, Sơn Nước, Ngói Lợp, Bồn Nước, Bình Nóng Lạnh Chính Hãng. Địa chỉ: 199 Xô Viết Nghệ Tĩnh, Cẩm Lệ, Đà Nẵng - Hotline: 0932.555.605">
    <meta property="og:image" content="https://placehold.co/1200x630/0f3e68/ffffff?text=MAI+BAO+CHAU+-+MINHHUY.COM">
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:image" content="https://placehold.co/1200x630/0f3e68/ffffff?text=MAI+BAO+CHAU+-+MINHHUY.COM">

    <!-- Google Fonts: Inter & Montserrat chuẩn giao diện Flatsome -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">

    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>

    <style>
        :root {
            --primary-color: #0f3e68;      /* Xanh đậm thương hiệu theo màu Logo */
            --primary-light: #1a568e;      /* Xanh sáng phụ trợ */
            --accent-color: #d97706;       /* Vàng cam điểm nhấn Logo */
            --sale-badge: #d26e4b;         /* Màu badge giảm giá góc trên trái chuẩn Flatsome */
            --price-color: #c81e1e;        /* Màu giá giảm nổi bật */
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        html, body {
            width: 100%;
            max-width: 100%;
            overflow-x: hidden;
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc;
            color: #1e293b;
            scroll-behavior: smooth;
        }

        /* Khung giao diện chuẩn Flatsome: Rộng 95% trên màn hình máy tính, căn giữa tuyệt đối, không lệch phải */
        .flatsome-container {
            width: 96%;
            max-width: 96%;
            margin-left: auto;
            margin-right: auto;
        }

        @media (min-width: 1024px) {
            .flatsome-container {
                width: 95%;
                max-width: 95%;
                margin-left: auto;
                margin-right: auto;
            }
        }

        /* Tối ưu thanh menu danh mục trên máy tính: chữ nhỏ gọn, viết liền trên 1 hàng, không bao giờ xuống dòng bên trong tên danh mục */
        .desktop-nav-list {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: flex-start;
            gap: 2px;
        }

        .desktop-nav-item {
            position: relative;
        }

        .desktop-nav-link {
            display: inline-flex;
            align-items: center;
            gap: 4px;
            padding: 9px 10px;
            font-size: 12px;
            font-weight: 700;
            color: #ffffff;
            text-transform: uppercase;
            white-space: nowrap; /* Tuyệt đối không xuống dòng tên danh mục */
            letter-spacing: 0.01em;
            transition: background-color 0.2s ease, color 0.2s ease;
            border-radius: 4px;
        }

        @media (min-width: 1280px) {
            .desktop-nav-link {
                padding: 10px 13px;
                font-size: 12.5px;
            }
        }

        .desktop-nav-link:hover,
        .desktop-nav-item:hover > .desktop-nav-link {
            background-color: rgba(255, 255, 255, 0.15);
            color: #fde68a;
        }

        /* Dropdown menu chuẩn Flatsome */
        .flatsome-dropdown {
            display: none;
            position: absolute;
            top: 100%;
            left: 0;
            min-width: 220px;
            background: #ffffff;
            border-top: 3px solid var(--accent-color);
            box-shadow: 0 10px 25px rgba(15, 62, 104, 0.16);
            border-radius: 0 0 8px 8px;
            z-index: 100;
            padding: 6px 0;
        }

        .desktop-nav-item:hover .flatsome-dropdown {
            display: block;
        }

        .flatsome-dropdown a {
            display: block;
            padding: 8px 14px;
            font-size: 12.5px;
            font-weight: 500;
            color: #334155;
            white-space: nowrap;
            border-bottom: 1px solid #f1f5f9;
            transition: all 0.15s ease;
        }

        .flatsome-dropdown a:last-child {
            border-bottom: none;
        }

        .flatsome-dropdown a:hover {
            background-color: #f0f7ff;
            color: var(--primary-color);
            padding-left: 18px;
        }

        /* Tiêu đề danh mục sản phẩm ở trang chủ nhỏ gọn, viết liền không gãy chữ */
        .section-cat-header {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: space-between;
            border-bottom: 2px solid var(--primary-color);
            background: #ffffff;
            border-radius: 8px 8px 0 0;
            margin-bottom: 12px;
            gap: 8px;
        }

        .section-cat-title {
            background: var(--primary-color);
            color: #ffffff;
            font-size: 13px;
            font-weight: 700;
            text-transform: uppercase;
            padding: 9px 16px;
            border-radius: 6px 6px 0 0;
            white-space: nowrap;
            display: inline-flex;
            align-items: center;
            gap: 7px;
        }

        .subcat-pills {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            gap: 4px;
            padding: 4px 10px;
        }

        .subcat-pill {
            font-size: 11.5px;
            font-weight: 600;
            color: #475569;
            padding: 4px 9px;
            border-radius: 4px;
            background: #f1f5f9;
            white-space: nowrap; /* Không xuống dòng tên danh mục con */
            transition: all 0.2s;
        }

        .subcat-pill:hover {
            background: var(--primary-color);
            color: #ffffff;
        }

        /* Thẻ sản phẩm chuẩn Flatsome Product Small Box */
        .product-small.box {
            background: #ffffff;
            border: 1px solid #e2e8f0;
            border-radius: 8px;
            overflow: hidden;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            position: relative;
            transition: transform 0.2s ease, box-shadow 0.2s ease;
            height: 100%;
        }

        .product-small.box:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(15, 62, 104, 0.1);
            border-color: #cbd5e1;
        }

        /* Badge % giảm giá chuẩn Flatsome góc trên bên trái */
        .badge-container.top.left {
            position: absolute;
            top: 8px;
            left: 8px;
            z-index: 10;
            pointer-events: none;
        }

        .onsale-badge {
            background-color: var(--sale-badge);
            color: #ffffff;
            font-size: 11px;
            font-weight: 700;
            width: 38px;
            height: 38px;
            border-radius: 9999px;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 2px 6px rgba(0, 0, 0, 0.18);
        }

        /* Tên sản phẩm đầy đủ, không bị cắt chữ hay tràn viền */
        .product-title-full {
            font-size: 13px;
            font-weight: 600;
            color: #1e293b;
            line-height: 1.4;
            word-break: break-word;
            overflow-wrap: anywhere;
            white-space: normal;
            margin-bottom: 6px;
        }

        /* 2 Banner tự trượt kích thước bằng nhau tuyệt đối */
        .banner-slider-viewport {
            position: relative;
            width: 100%;
            height: 320px;
            border-radius: 10px;
            overflow: hidden;
        }

        @media (min-width: 640px) {
            .banner-slider-viewport {
                height: 350px;
            }
        }

        @media (min-width: 1024px) {
            .banner-slider-viewport {
                height: 390px;
            }
        }

        .banner-slide {
            position: absolute;
            inset: 0;
            width: 100%;
            height: 100%;
            opacity: 0;
            visibility: hidden;
            transition: opacity 0.6s ease-in-out, visibility 0.6s ease-in-out;
        }

        .banner-slide.active {
            opacity: 1;
            visibility: visible;
            z-index: 5;
        }

        /* Nút liên hệ nổi bật tương thích điện thoại & máy tính */
        @keyframes pulse-ring {
            0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(217, 119, 6, 0.7); }
            70% { transform: scale(1); box-shadow: 0 0 0 10px rgba(217, 119, 6, 0); }
            100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(217, 119, 6, 0); }
        }

        .floating-btn-pulse {
            animation: pulse-ring 2s infinite;
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800">

    <!-- ==========================================
         HEADER FLATSOME (#header)
         Lưu ý: Không để nút gọi ngay trên Header để tránh tràn viền
    =========================================== -->
    <header id="header" class="header w-full bg-white shadow-sm sticky top-0 z-50">
        <div class="header-wrapper">

            <!-- Top Bar (#top-bar) -->
            <div id="top-bar" class="header-top bg-[#0a2c4d] text-white text-xs py-1.5">
                <div class="flatsome-container flex flex-wrap items-center justify-between gap-2">
                    <div class="flex items-center gap-2 truncate">
                        <span class="font-semibold text-amber-300">CÔNG TY TNHH MAI BẢO CHÂU</span>
                        <span class="hidden sm:inline text-slate-300">|</span>
                        <span class="hidden sm:inline text-slate-200"><i class="fa-solid fa-location-dot text-amber-400 mr-1"></i>199 Xô Viết Nghệ Tĩnh, Cẩm Lệ, Đà Nẵng</span>
                    </div>
                    <div class="flex items-center gap-3 text-[11.5px] whitespace-nowrap">
                        <a href="#gioi-thieu-cua-hang" class="hover:text-amber-300 transition">Giới thiệu</a>
                        <span class="text-slate-400">|</span>
                        <a href="#anh-thuc-te" class="hover:text-amber-300 transition">Hình ảnh thực tế</a>
                        <span class="text-slate-400">|</span>
                        <a href="#tin-tuc" class="hover:text-amber-300 transition">Tin tức</a>
                        <span class="text-slate-400">|</span>
                        <a href="#lien-he-bando" class="hover:text-amber-300 transition">Liên hệ</a>
                    </div>
                </div>
            </div>

            <!-- Main Header (#masthead): Logo nhỏ gọn + Tìm kiếm + Giỏ báo giá (Không có nút gọi ngay tránh tràn viền) -->
            <div id="masthead" class="header-main py-2.5 bg-white border-b border-slate-100">
                <div class="flatsome-container flex items-center justify-between gap-3">

                    <!-- Nút mở Menu trên Điện thoại -->
                    <button id="mobile-menu-btn" type="button" aria-label="Mở danh mục" class="lg:hidden p-2 rounded-md border border-slate-200 text-[#0f3e68] hover:bg-slate-100 shrink-0">
                        <i class="fa-solid fa-bars text-lg"></i>
                    </button>

                    <!-- Logo Công Ty TNHH Mai Bảo Châu - minhhuy.com (Thiết kế gọn nhỏ, sắc nét) -->
                    <a href="#" class="flex items-center gap-2.5 shrink-0 group">
                        <svg class="w-10 h-10 sm:w-11 sm:h-11 shrink-0 rounded-lg shadow-sm" viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
                            <defs>
                                <linearGradient id="logoGrad" x1="0%" y1="0%" x2="100%" y2="100%">
                                    <stop offset="0%" stop-color="#0f3e68" />
                                    <stop offset="100%" stop-color="#1e5b94" />
                                </linearGradient>
                            </defs>
                            <rect width="100" height="100" rx="18" fill="url(#logoGrad)" />
                            <!-- Biểu tượng Mái nhà & Viên gạch VLXD -->
                            <path d="M18 46 L50 20 L82 46 L74 46 L50 27 L26 46 Z" fill="#f59e0b" />
                            <rect x="29" y="48" width="19" height="19" rx="3" fill="#ffffff" />
                            <rect x="52" y="48" width="19" height="19" rx="3" fill="#fbbf24" />
                            <text x="50" y="85" font-family="Inter, sans-serif" font-size="14" font-weight="800" fill="#ffffff" text-anchor="middle">MBC</text>
                        </svg>
                        <div class="leading-tight">
                            <div class="text-xs sm:text-sm md:text-base font-extrabold text-[#0f3e68] tracking-tight">
                                CÔNG TY TNHH MAI BẢO CHÂU
                            </div>
                            <div class="text-[11px] sm:text-xs font-bold text-amber-600 flex items-center gap-1.5">
                                <span>SHOWROOM MINH HUY</span>
                                <span class="text-slate-300">•</span>
                                <span class="text-[#0f3e68] underline">minhhuy.com</span>
                            </div>
                        </div>
                    </a>

                    <!-- Ô tìm kiếm sản phẩm ở giữa -->
                    <div class="hidden md:flex flex-1 max-w-xl mx-2">
                        <form id="header-search-form" class="w-full flex items-center border-2 border-[#0f3e68] rounded-md overflow-hidden bg-slate-50" onsubmit="handleProductSearch(event)">
                            <input id="header-search-input" type="text" placeholder="Tìm sơn Jotun, bồn cầu Inax, gạch men Đồng Tâm, ngói lợp, bồn nước..." class="w-full px-3 py-1.5 text-xs sm:text-sm bg-transparent focus:outline-none text-slate-700">
                            <button type="submit" class="bg-[#0f3e68] hover:bg-[#1a568e] text-white px-4 py-2 text-xs font-semibold transition shrink-0">
                                <i class="fa-solid fa-magnifying-glass mr-1"></i>Tìm
                            </button>
                        </form>
                    </div>

                    <!-- Liên kết nhanh tới Form Báo Giá (Nhỏ gọn, không tràn viền) -->
                    <div class="flex items-center gap-2 shrink-0">
                        <a href="#form-bao-gia" class="inline-flex items-center gap-1.5 bg-amber-500 hover:bg-amber-600 text-white text-xs font-bold px-3 py-2 rounded-md shadow-sm transition whitespace-nowrap">
                            <i class="fa-solid fa-file-invoice-dollar"></i>
                            <span>Nhận Báo Giá</span>
                        </a>
                    </div>
                </div>

                <!-- Thanh tìm kiếm trên điện thoại -->
                <div class="flatsome-container md:hidden mt-2">
                    <form class="w-full flex items-center border border-[#0f3e68] rounded-md overflow-hidden bg-slate-50" onsubmit="handleProductSearch(event)">
                        <input id="mobile-search-input" type="text" placeholder="Tìm kiếm sản phẩm tại minhhuy.com..." class="w-full px-3 py-1.5 text-xs bg-transparent focus:outline-none">
                        <button type="submit" class="bg-[#0f3e68] text-white px-3 py-1.5 text-xs font-semibold shrink-0">
                            <i class="fa-solid fa-magnifying-glass"></i>
                        </button>
                    </form>
                </div>
            </div>

            <!-- Thanh Menu Danh Mục Máy Tính (#wide-nav): Chữ nhỏ gọn, nằm liền trên 1 hàng, không gãy dòng -->
            <div id="wide-nav" class="header-bottom bg-[#0f3e68] hidden lg:block">
                <div class="flatsome-container">
                    <ul class="desktop-nav-list">
                        <li class="desktop-nav-item">
                            <a href="#" class="desktop-nav-link bg-amber-600 text-white"><i class="fa-solid fa-house"></i>TRANG CHỦ</a>
                        </li>
                        <li class="desktop-nav-item">
                            <a href="#cat-son" class="desktop-nav-link">SƠN <i class="fa-solid fa-angle-down text-[10px]"></i></a>
                            <div class="flatsome-dropdown">
                                <a href="#cat-son">Sơn Jotun (Nội & Ngoại Thất)</a>
                                <a href="#cat-son">Sơn Dulux - Maxilite</a>
                                <a href="#cat-son">Sơn Tito Chống Thấm & Sơn Nhũ</a>
                                <a href="#cat-son">Chống Thấm Sika / Bestmix / Mapei</a>
                            </div>
                        </li>
                        <li class="desktop-nav-item">
                            <a href="#cat-tbvs" class="desktop-nav-link">THIẾT BỊ VỆ SINH <i class="fa-solid fa-angle-down text-[10px]"></i></a>
                            <div class="flatsome-dropdown">
                                <a href="#cat-tbvs">Bồn Cầu Inax / Viglacera / Caesar</a>
                                <a href="#cat-tbvs">Sen Vòi & Sen Cây Nóng Lạnh</a>
                                <a href="#cat-tbvs">Chậu Rửa Lavabo</a>
                                <a href="#cat-tbvs">Gương Phòng Tắm</a>
                                <a href="#cat-tbvs">Phụ Kiện Nhà Tắm</a>
                            </div>
                        </li>
                        <li class="desktop-nav-item">
                            <a href="#cat-gach-men" class="desktop-nav-link">GẠCH MEN <i class="fa-solid fa-angle-down text-[10px]"></i></a>
                            <div class="flatsome-dropdown">
                                <a href="#cat-gach-men">Gạch Đồng Tâm (80x80, 60x60, 40x80)</a>
                                <a href="#cat-gach-men">Gạch Đồng Tâm (40x40, 30x60)</a>
                                <a href="#cat-gach-men">Gạch Kimgres Cao Cấp</a>
                            </div>
                        </li>
                        <li class="desktop-nav-item">
                            <a href="#cat-ngoi-lop" class="desktop-nav-link">NGÓI LỢP <i class="fa-solid fa-angle-down text-[10px]"></i></a>
                            <div class="flatsome-dropdown">
                                <a href="#cat-ngoi-lop">Ngói Lợp DIC</a>
                                <a href="#cat-ngoi-lop">Ngói Đất Việt</a>
                                <a href="#cat-ngoi-lop">Ngói Màu Sunrise</a>
                            </div>
                        </li>
                        <li class="desktop-nav-item">
                            <a href="#cat-bon-nuoc" class="desktop-nav-link">BỒN NƯỚC <i class="fa-solid fa-angle-down text-[10px]"></i></a>
                            <div class="flatsome-dropdown">
                                <a href="#cat-bon-nuoc">Bồn Nước Letton</a>
                                <a href="#cat-bon-nuoc">Bồn Nước Sơn Hà</a>
                                <a href="#cat-bon-nuoc">Bồn Nước Tân Á Đại Thành</a>
                            </div>
                        </li>
                        <li class="desktop-nav-item">
                            <a href="#cat-binh-nong-lanh" class="desktop-nav-link">BÌNH NÓNG LẠNH <i class="fa-solid fa-angle-down text-[10px]"></i></a>
                            <div class="flatsome-dropdown">
                                <a href="#cat-binh-nong-lanh">Bình Nóng Lạnh Ariston</a>
                                <a href="#cat-binh-nong-lanh">Bình Nóng Lạnh Ferroli</a>
                            </div>
                        </li>
                        <li class="desktop-nav-item">
                            <a href="#cat-keo-dan-gach" class="desktop-nav-link">DÁN GẠCH, CHÀ RON <i class="fa-solid fa-angle-down text-[10px]"></i></a>
                            <div class="flatsome-dropdown">
                                <a href="#cat-keo-dan-gach">Keo Dán Gạch Bestmix</a>
                                <a href="#cat-keo-dan-gach">Keo Chà Ron Đồng Tâm</a>
                                <a href="#cat-keo-dan-gach">Keo Cá Sấu (Crocodile)</a>
                                <a href="#cat-keo-dan-gach">Vữa & Keo Sika</a>
                            </div>
                        </li>
                        <li class="desktop-nav-item">
                            <a href="#anh-thuc-te" class="desktop-nav-link">ẢNH THỰC TẾ</a>
                        </li>
                        <li class="desktop-nav-item">
                            <a href="#doi-tac" class="desktop-nav-link">ĐỐI TÁC</a>
                        </li>
                        <li class="desktop-nav-item">
                            <a href="#tin-tuc" class="desktop-nav-link">BÀI VIẾT</a>
                        </li>
                        <li class="desktop-nav-item">
                            <a href="#lien-he-bando" class="desktop-nav-link">LIÊN HỆ</a>
                        </li>
                    </ul>
                </div>
            </div>

            <!-- Danh mục cuộn ngang nhanh trên Điện thoại (Nhỏ gọn, đẹp mắt, không tràn viền) -->
            <div class="lg:hidden bg-[#0f3e68] text-white border-t border-white/10">
                <div class="flatsome-container py-1.5 flex items-center gap-1.5 overflow-x-auto no-scrollbar">
                    <a href="#cat-son" class="px-2.5 py-1 rounded bg-white/10 text-[11px] font-semibold whitespace-nowrap">SƠN</a>
                    <a href="#cat-tbvs" class="px-2.5 py-1 rounded bg-white/10 text-[11px] font-semibold whitespace-nowrap">THIẾT BỊ VỆ SINH</a>
                    <a href="#cat-gach-men" class="px-2.5 py-1 rounded bg-white/10 text-[11px] font-semibold whitespace-nowrap">GẠCH MEN</a>
                    <a href="#cat-ngoi-lop" class="px-2.5 py-1 rounded bg-white/10 text-[11px] font-semibold whitespace-nowrap">NGÓI LỢP</a>
                    <a href="#cat-bon-nuoc" class="px-2.5 py-1 rounded bg-white/10 text-[11px] font-semibold whitespace-nowrap">BỒN NƯỚC</a>
                    <a href="#cat-binh-nong-lanh" class="px-2.5 py-1 rounded bg-white/10 text-[11px] font-semibold whitespace-nowrap">BÌNH NÓNG LẠNH</a>
                    <a href="#cat-keo-dan-gach" class="px-2.5 py-1 rounded bg-white/10 text-[11px] font-semibold whitespace-nowrap">DÁN GẠCH, CHÀ RON</a>
                </div>
            </div>
        </div>
    </header>

    <!-- Menu Drawer trên Điện thoại -->
    <div id="mobile-drawer" class="fixed inset-0 bg-black/60 z-50 hidden">
        <div class="w-72 max-w-[85vw] bg-white h-full shadow-2xl flex flex-col justify-between overflow-y-auto">
            <div>
                <div class="p-4 bg-[#0f3e68] text-white flex items-center justify-between">
                    <span class="font-bold text-sm">DANH MỤC MINHHUY.COM</span>
                    <button id="close-mobile-menu" type="button" class="w-8 h-8 rounded bg-white/10 flex items-center justify-center">
                        <i class="fa-solid fa-xmark"></i>
                    </button>
                </div>
                <nav class="divide-y divide-slate-100 text-xs font-semibold text-slate-700">
                    <a href="#" onclick="closeMobileMenu()" class="block px-4 py-3 hover:bg-slate-50 text-[#0f3e68]">TRANG CHỦ</a>
                    <a href="#cat-son" onclick="closeMobileMenu()" class="block px-4 py-3 hover:bg-slate-50">SƠN (Jotun, Dulux, Tito, Chống thấm)</a>
                    <a href="#cat-tbvs" onclick="closeMobileMenu()" class="block px-4 py-3 hover:bg-slate-50">THIẾT BỊ VỆ SINH (Bồn cầu, Sen vòi, Lavabo)</a>
                    <a href="#cat-gach-men" onclick="closeMobileMenu()" class="block px-4 py-3 hover:bg-slate-50">GẠCH MEN (Đồng Tâm, Kimgres)</a>
                    <a href="#cat-ngoi-lop" onclick="closeMobileMenu()" class="block px-4 py-3 hover:bg-slate-50">NGÓI LỢP (DIC, Ngói Đất Việt)</a>
                    <a href="#cat-bon-nuoc" onclick="closeMobileMenu()" class="block px-4 py-3 hover:bg-slate-50">BỒN NƯỚC (Letton, Sơn Hà, Tân Á)</a>
                    <a href="#cat-binh-nong-lanh" onclick="closeMobileMenu()" class="block px-4 py-3 hover:bg-slate-50">BÌNH NÓNG LẠNH (Ariston, Ferroli)</a>
                    <a href="#cat-keo-dan-gach" onclick="closeMobileMenu()" class="block px-4 py-3 hover:bg-slate-50">KEO DÁN GẠCH, CHÀ RON</a>
                    <a href="#anh-thuc-te" onclick="closeMobileMenu()" class="block px-4 py-3 hover:bg-slate-50">HÌNH ẢNH THỰC TẾ SẢN PHẨM & CỬA HÀNG</a>
                    <a href="#doi-tac" onclick="closeMobileMenu()" class="block px-4 py-3 hover:bg-slate-50">ĐỐI TÁC THƯƠNG HIỆU</a>
                    <a href="#tin-tuc" onclick="closeMobileMenu()" class="block px-4 py-3 hover:bg-slate-50">TIN TỨC & CẨM NANG</a>
                    <a href="#form-bao-gia" onclick="closeMobileMenu()" class="block px-4 py-3 hover:bg-slate-50">YÊU CẦU BÁO GIÁ</a>
                    <a href="#lien-he-bando" onclick="closeMobileMenu()" class="block px-4 py-3 hover:bg-slate-50">BẢN ĐỒ & FANPAGE</a>
                </nav>
            </div>
            <div class="p-4 bg-slate-50 border-t border-slate-200 text-xs space-y-1">
                <div class="font-bold text-[#0f3e68]">CÔNG TY TNHH MAI BẢO CHÂU</div>
                <div>Đ/c: 199 Xô Viết Nghệ Tĩnh, Cẩm Lệ, Đà Nẵng</div>
                <div class="font-bold text-red-600">Hotline/Zalo: 0932.555.605</div>
            </div>
        </div>
    </div>

    <!-- ==========================================
         MAIN CONTENT (#main) - CẤU TRÚC UX BUILDER FLATSOME
    =========================================== -->
    <main id="main" class="py-4 space-y-6">

        <!-- SECTION 1: 2 ẢNH BANNER TỰ TRƯỢT KÍCH THƯỚC BẰNG NHAU
             Hình ảnh & chữ nằm trọn trong banner, chữ cách xa viền, không bị thiếu chữ trên cả ĐT & Máy tính -->
        <section class="section-banner">
            <div class="flatsome-container">
                <div class="banner-slider-viewport shadow-md">

                    <!-- SLIDE 1 -->
                    <div class="banner-slide active bg-gradient-to-r from-[#0a2c4d] via-[#0f3e68] to-[#1e5b94]">
                        <!-- Khoảng đệm an toàn (px-7 sm:px-14 lg:px-20 py-6) giúp chữ luôn cách xa viền banner -->
                        <div class="w-full h-full px-7 sm:px-14 lg:px-20 py-6 flex flex-col md:flex-row items-center justify-between gap-4">
                            <div class="w-full md:w-3/5 text-white space-y-2 sm:space-y-3 text-center md:text-left">
                                <div class="text-amber-300 text-xs sm:text-sm font-bold tracking-wider uppercase">
                                    CÔNG TY TNHH MAI BẢO CHÂU • MINHHUY.COM
                                </div>
                                <h1 class="text-base sm:text-2xl lg:text-3xl font-extrabold leading-snug">
                                    TRUNG TÂM PHÂN PHỐI GẠCH MEN, THIẾT BỊ VỆ SINH & SƠN CHÍNH HÃNG
                                </h1>
                                <p class="text-xs sm:text-sm text-slate-200 leading-relaxed">
                                    Chuyên cung cấp Sỉ & Lẻ Thiết bị vệ sinh INAX, Viglacera, Gạch men Đồng Tâm, Kimgres, Sơn Jotun, Dulux uy tín tại Đà Nẵng.
                                </p>
                                <div class="pt-1 flex flex-wrap items-center justify-center md:justify-start gap-2 text-xs sm:text-sm font-semibold text-amber-200">
                                    <span><i class="fa-solid fa-location-dot mr-1"></i>199 Xô Viết Nghệ Tĩnh, Cẩm Lệ, Đà Nẵng</span>
                                    <span class="hidden sm:inline">•</span>
                                    <span><i class="fa-solid fa-phone-volume mr-1"></i>0932.555.605</span>
                                </div>
                            </div>
                            <!-- Hình ảnh sản phẩm nằm gọn bên trong Banner 1 -->
                            <div class="w-full md:w-2/5 flex items-center justify-center gap-2 sm:gap-3">
                                <img src="https://drive.google.com/thumbnail?id=1DaeFx6AXIb9EdOjTVr2EcVqQD7k-q1Ns&sz=w600"
                                     onerror="this.onerror=null;this.src='https://placehold.co/320x220/1e5b94/ffffff?text=Showroom+Minh+Huy';"
                                     alt="Cửa hàng Mai Bảo Châu - Minh Huy"
                                     class="w-36 sm:w-44 lg:w-52 h-24 sm:h-36 lg:h-44 object-cover rounded-lg border-2 border-amber-400/70 shadow-lg bg-white">
                                <img src="https://drive.google.com/thumbnail?id=1P2fePSvPXm6YIcNDixVa0YwFWshcHFDY&sz=w600"
                                     onerror="this.onerror=null;this.src='https://placehold.co/320x220/1e5b94/ffffff?text=San+Pham+Minh+Huy';"
                                     alt="Sản phẩm thực tế Mai Bảo Châu"
                                     class="w-36 sm:w-44 lg:w-52 h-24 sm:h-36 lg:h-44 object-cover rounded-lg border-2 border-white/60 shadow-lg bg-white">
                            </div>
                        </div>
                    </div>

                    <!-- SLIDE 2 -->
                    <div class="banner-slide bg-gradient-to-r from-[#133b5c] via-[#1d5685] to-[#0f3e68]">
                        <!-- Khoảng đệm an toàn giúp chữ luôn cách xa viền banner -->
                        <div class="w-full h-full px-7 sm:px-14 lg:px-20 py-6 flex flex-col md:flex-row items-center justify-between gap-4">
                            <div class="w-full md:w-3/5 text-white space-y-2 sm:space-y-3 text-center md:text-left">
                                <div class="text-amber-300 text-xs sm:text-sm font-bold tracking-wider uppercase">
                                    SHOWROOM VẬT LIỆU XÂY DỰNG & NỘI NGOẠI THẤT MINH HUY
                                </div>
                                <h2 class="text-base sm:text-2xl lg:text-3xl font-extrabold leading-snug">
                                    ĐẠI LÝ NGÓI LỢP, BỒN NƯỚC, BÌNH NÓNG LẠNH & KEO DÁN GẠCH GIÁ SỈ
                                </h2>
                                <p class="text-xs sm:text-sm text-slate-200 leading-relaxed">
                                    Phân phối chính hãng Bồn nước Tân Á, Sơn Hà, Bình nóng lạnh Ariston, Ferroli, Ngói lợp DIC, Đất Việt, Chống thấm Sika chiết khấu cao.
                                </p>
                                <div class="pt-1 flex flex-wrap items-center justify-center md:justify-start gap-2 text-xs sm:text-sm font-semibold text-amber-200">
                                    <span><i class="fa-solid fa-globe mr-1"></i>Website: minhhuy.com</span>
                                    <span class="hidden sm:inline">•</span>
                                    <span><i class="fa-solid fa-headset mr-1"></i>Tư vấn & Giao hàng tận công trình: 0932.555.605</span>
                                </div>
                            </div>
                            <!-- Hình ảnh sản phẩm nằm gọn bên trong Banner 2 -->
                            <div class="w-full md:w-2/5 flex items-center justify-center gap-2 sm:gap-3">
                                <img src="https://drive.google.com/thumbnail?id=11z7ir7cmqEcdrYuAThZvpOhgUVFsLUnP&sz=w600"
                                     onerror="this.onerror=null;this.src='https://placehold.co/320x220/0f3e68/ffffff?text=Thiet+Bi+Ve+Sinh';"
                                     alt="Thiết bị vệ sinh Minh Huy"
                                     class="w-36 sm:w-44 lg:w-52 h-24 sm:h-36 lg:h-44 object-cover rounded-lg border-2 border-amber-400/70 shadow-lg bg-white">
                                <img src="https://drive.google.com/thumbnail?id=1KTDzdSGqiXWuLZDkPoDD7oZZVL-5F3Rr&sz=w600"
                                     onerror="this.onerror=null;this.src='https://placehold.co/320x220/0f3e68/ffffff?text=Gach+Men+Cao+Cap';"
                                     alt="Vật liệu xây dựng Minh Huy"
                                     class="w-36 sm:w-44 lg:w-52 h-24 sm:h-36 lg:h-44 object-cover rounded-lg border-2 border-white/60 shadow-lg bg-white">
                            </div>
                        </div>
                    </div>

                    <!-- Nút điều hướng qua lại & Chấm tròn chỉ báo Slide -->
                    <button type="button" onclick="changeBannerSlide(-1)" aria-label="Slide trước" class="absolute left-2 top-1/2 -translate-y-1/2 z-10 w-8 h-8 rounded-full bg-black/35 hover:bg-black/60 text-white flex items-center justify-center transition">
                        <i class="fa-solid fa-chevron-left text-xs"></i>
                    </button>
                    <button type="button" onclick="changeBannerSlide(1)" aria-label="Slide tiếp" class="absolute right-2 top-1/2 -translate-y-1/2 z-10 w-8 h-8 rounded-full bg-black/35 hover:bg-black/60 text-white flex items-center justify-center transition">
                        <i class="fa-solid fa-chevron-right text-xs"></i>
                    </button>
                    <div class="absolute bottom-2.5 left-1/2 -translate-x-1/2 z-10 flex items-center gap-2">
                        <button type="button" onclick="goToBannerSlide(0)" class="banner-dot w-2.5 h-2.5 rounded-full bg-amber-400 transition"></button>
                        <button type="button" onclick="goToBannerSlide(1)" class="banner-dot w-2.5 h-2.5 rounded-full bg-white/50 transition"></button>
                    </div>
                </div>
            </div>
        </section>

        <!-- SECTION 2: DANH MỤC SẢN PHẨM TRANG CHỦ (Chữ nhỏ gọn, không xuống dòng tên danh mục, đẹp trên cả máy tính & ĐT) -->
        <section class="section-home-categories">
            <div class="flatsome-container">
                <div class="bg-white p-3.5 sm:p-4 rounded-lg border border-slate-200 shadow-sm">
                    <div class="flex items-center justify-between mb-3 pb-2 border-b border-slate-100">
                        <h2 class="text-xs sm:text-sm font-extrabold text-[#0f3e68] uppercase tracking-wide">
                            <i class="fa-solid fa-layer-group text-amber-600 mr-1.5"></i>DANH MỤC SẢN PHẨM CHÍNH HÃNG
                        </h2>
                        <span class="text-[11px] text-slate-500 hidden sm:inline">Chọn nhanh danh mục vật tư công trình</span>
                    </div>
                    <div class="grid grid-cols-2 sm:grid-cols-4 lg:grid-cols-7 gap-2.5">
                        <a href="#cat-son" class="flex items-center gap-2 p-2.5 rounded-md bg-slate-50 hover:bg-[#0f3e68] hover:text-white border border-slate-200 transition group">
                            <i class="fa-solid fa-fill-drip text-[#0f3e68] group-hover:text-amber-300 text-sm shrink-0"></i>
                            <span class="text-xs font-bold whitespace-nowrap">SƠN NƯỚC</span>
                        </a>
                        <a href="#cat-tbvs" class="flex items-center gap-2 p-2.5 rounded-md bg-slate-50 hover:bg-[#0f3e68] hover:text-white border border-slate-200 transition group">
                            <i class="fa-solid fa-shower text-[#0f3e68] group-hover:text-amber-300 text-sm shrink-0"></i>
                            <span class="text-xs font-bold whitespace-nowrap">THIẾT BỊ VỆ SINH</span>
                        </a>
                        <a href="#cat-gach-men" class="flex items-center gap-2 p-2.5 rounded-md bg-slate-50 hover:bg-[#0f3e68] hover:text-white border border-slate-200 transition group">
                            <i class="fa-solid fa-border-all text-[#0f3e68] group-hover:text-amber-300 text-sm shrink-0"></i>
                            <span class="text-xs font-bold whitespace-nowrap">GẠCH MEN</span>
                        </a>
                        <a href="#cat-ngoi-lop" class="flex items-center gap-2 p-2.5 rounded-md bg-slate-50 hover:bg-[#0f3e68] hover:text-white border border-slate-200 transition group">
                            <i class="fa-solid fa-house-chimney text-[#0f3e68] group-hover:text-amber-300 text-sm shrink-0"></i>
                            <span class="text-xs font-bold whitespace-nowrap">NGÓI LỢP</span>
                        </a>
                        <a href="#cat-bon-nuoc" class="flex items-center gap-2 p-2.5 rounded-md bg-slate-50 hover:bg-[#0f3e68] hover:text-white border border-slate-200 transition group">
                            <i class="fa-solid fa-database text-[#0f3e68] group-hover:text-amber-300 text-sm shrink-0"></i>
                            <span class="text-xs font-bold whitespace-nowrap">BỒN NƯỚC</span>
                        </a>
                        <a href="#cat-binh-nong-lanh" class="flex items-center gap-2 p-2.5 rounded-md bg-slate-50 hover:bg-[#0f3e68] hover:text-white border border-slate-200 transition group">
                            <i class="fa-solid fa-temperature-arrow-up text-[#0f3e68] group-hover:text-amber-300 text-sm shrink-0"></i>
                            <span class="text-xs font-bold whitespace-nowrap">BÌNH NÓNG LẠNH</span>
                        </a>
                        <a href="#cat-keo-dan-gach" class="flex items-center gap-2 p-2.5 rounded-md bg-slate-50 hover:bg-[#0f3e68] hover:text-white border border-slate-200 transition group col-span-2 sm:col-span-1">
                            <i class="fa-solid fa-trowel-bricks text-[#0f3e68] group-hover:text-amber-300 text-sm shrink-0"></i>
                            <span class="text-xs font-bold whitespace-nowrap">DÁN GẠCH, CHÀ RON</span>
                        </a>
                    </div>
                </div>
            </div>
        </section>

        <!-- SECTION 3: GIỚI THIỆU CỬA HÀNG & 19 ẢNH SẢN PHẨM THỰC TẾ TRONG FILE GOOGLE DRIVE
             Tích hợp đầy đủ ảnh cửa hàng + 19 ảnh thực tế, chia 2 cột trên điện thoại, có % giảm giá góc trên trái chuẩn Flatsome -->
        <section id="anh-thuc-te" class="section-real-drive-products">
            <div class="flatsome-container space-y-4">

                <!-- Khung Giới Thiệu Công Ty TNHH Mai Bảo Châu & Ảnh Cửa Hàng Thực Tế -->
                <div id="gioi-thieu-cua-hang" class="bg-white rounded-lg border border-slate-200 p-4 sm:p-5 shadow-sm">
                    <div class="grid grid-cols-1 lg:grid-cols-12 gap-5 items-center">
                        <div class="lg:col-span-5">
                            <a href="https://drive.google.com/file/d/1DaeFx6AXIb9EdOjTVr2EcVqQD7k-q1Ns/view?usp=sharing" target="_blank" rel="noopener" class="block rounded-lg overflow-hidden border border-slate-200 shadow-sm">
                                <img src="https://drive.google.com/thumbnail?id=1DaeFx6AXIb9EdOjTVr2EcVqQD7k-q1Ns&sz=w1000"
                                     onerror="this.onerror=null;this.src='https://lh3.googleusercontent.com/d/1DaeFx6AXIb9EdOjTVr2EcVqQD7k-q1Ns=w1000';"
                                     alt="Ảnh cửa hàng Công Ty TNHH Mai Bảo Châu - 199 Xô Viết Nghệ Tĩnh"
                                     class="w-full h-56 sm:h-64 object-cover">
                            </a>
                        </div>
                        <div class="lg:col-span-7 space-y-2.5">
                            <div class="text-xs font-bold text-amber-600 uppercase">SHOWROOM VẬT LIỆU XÂY DỰNG & NỘI NGOẠI THẤT UY TÍN TẠI ĐÀ NẴNG</div>
                            <h2 class="text-lg sm:text-xl font-extrabold text-[#0f3e68]">
                                CÔNG TY TNHH MAI BẢO CHÂU – SHOWROOM MINH HUY (MINHHUY.COM)
                            </h2>
                            <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
                                Tọa lạc tại <strong>199 Xô Viết Nghệ Tĩnh, Quận Cẩm Lệ, TP. Đà Nẵng</strong>, <strong>Công Ty TNHH Mai Bảo Châu (Showroom Minh Huy)</strong> chuyên phân phối sỉ & lẻ Sơn nước nội ngoại thất (Jotun, Dulux, Maxilite, Tito), Thiết bị vệ sinh cao cấp (INAX, Viglacera, Caesar), Gạch men ốp lát (Đồng Tâm, Kimgres), Ngói lợp (DIC, Đất Việt, Sunrise), Bồn nước Inox & Nhựa (Tân Á, Sơn Hà, Letton), Bình nóng lạnh (Ariston, Ferroli), Vật liệu chống thấm & Keo dán gạch (Sika, Bestmix, Keo cá sấu) cùng thiết bị điện, đèn trang trí.
                            </p>
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-2 pt-1 text-xs">
                                <div class="p-2.5 rounded bg-slate-50 border border-slate-200">
                                    <i class="fa-solid fa-location-dot text-[#0f3e68] mr-1.5"></i><strong>Địa chỉ:</strong> 199 Xô Viết Nghệ Tĩnh, Cẩm Lệ, Đà Nẵng
                                </div>
                                <div class="p-2.5 rounded bg-slate-50 border border-slate-200">
                                    <i class="fa-solid fa-phone text-red-600 mr-1.5"></i><strong>Điện thoại / Zalo:</strong> <a href="tel:0932555605" class="font-bold text-red-600">0932.555.605</a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Danh sách 19 sản phẩm thực tế tại Showroom (từ 19 link Google Drive) -->
                <div>
                    <div class="section-cat-header">
                        <h2 class="section-cat-title">
                            <i class="fa-solid fa-camera"></i>SẢN PHẨM THỰC TẾ TẠI SHOWROOM MAI BẢO CHÂU
                        </h2>
                        <div class="subcat-pills">
                            <a href="#cat-tbvs" class="subcat-pill">Thiết bị vệ sinh</a>
                            <a href="#cat-gach-men" class="subcat-pill">Gạch men</a>
                            <a href="#cat-son" class="subcat-pill">Sơn & Chống thấm</a>
                            <a href="#cat-bon-nuoc" class="subcat-pill">Bồn nước & Nóng lạnh</a>
                        </div>
                    </div>
                    <!-- Grid sản phẩm: 2 cột trên điện thoại (grid-cols-2), 4-5 cột trên máy tính -->
                    <div id="drive-products-grid" class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-5 gap-3 sm:gap-4"></div>
                </div>

            </div>
        </section>

        <!-- SECTION 4: CÁC DANH MỤC SẢN PHẨM CHUẨN WEB MẪU NOITHATNGONGUYEN.COM -->
        <div id="catalog-sections-container" class="space-y-6"></div>

        <!-- SECTION 5: FORM YÊU CẦU VÀ NHẬN BÁO GIÁ TRANG CHỦ -->
        <section id="form-bao-gia" class="section-quote-form">
            <div class="flatsome-container">
                <div class="bg-gradient-to-br from-[#0f3e68] to-[#1a568e] rounded-xl p-5 sm:p-7 text-white shadow-md">
                    <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 items-center">
                        <div class="lg:col-span-5 space-y-3">
                            <div class="text-xs font-bold uppercase text-amber-300 tracking-wider">HỖ TRỢ CHỦ NHÀ & NHÀ THẦU XÂY DỰNG</div>
                            <h2 class="text-lg sm:text-2xl font-extrabold leading-snug">
                                ĐĂNG KÝ YÊU CẦU TƯ VẤN & NHẬN BÁO GIÁ VẬT LIỆU XÂY DỰNG
                            </h2>
                            <p class="text-xs sm:text-sm text-slate-200 leading-relaxed">
                                Quý khách hàng, nhà thầu, kỹ sư cần bảng báo giá chiết khấu tốt nhất các hạng mục Sơn, Thiết bị vệ sinh, Gạch men, Ngói lợp, Bồn nước, Bình nóng lạnh, Keo dán gạch tại <strong>Công Ty TNHH Mai Bảo Châu (minhhuy.com)</strong> vui lòng điền thông tin bên cạnh.
                            </p>
                            <div class="space-y-1.5 text-xs sm:text-sm pt-1">
                                <div><i class="fa-solid fa-circle-check text-amber-400 mr-2"></i>Cam kết hàng chính hãng 100% từ nhà máy</div>
                                <div><i class="fa-solid fa-circle-check text-amber-400 mr-2"></i>Chiết khấu cao cho công trình nhà phố, biệt thự, dự án</div>
                                <div><i class="fa-solid fa-circle-check text-amber-400 mr-2"></i>Giao hàng nhanh tận chân công trình tại Đà Nẵng & Miền Trung</div>
                            </div>
                        </div>

                        <div class="lg:col-span-7 bg-white text-slate-800 rounded-lg p-4 sm:p-6 shadow-lg">
                            <form id="quote-request-form" onsubmit="submitQuoteForm(event)" class="space-y-3">
                                <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                                    <div>
                                        <label class="block text-xs font-bold text-slate-700 mb-1">Họ và tên quý khách *</label>
                                        <input id="quote-name" type="text" required placeholder="Nhập họ và tên..." class="w-full px-3 py-2 text-xs sm:text-sm border border-slate-300 rounded focus:outline-none focus:border-[#0f3e68]">
                                    </div>
                                    <div>
                                        <label class="block text-xs font-bold text-slate-700 mb-1">Số điện thoại / Zalo *</label>
                                        <input id="quote-phone" type="tel" required placeholder="Ví dụ: 0932.555.605" class="w-full px-3 py-2 text-xs sm:text-sm border border-slate-300 rounded focus:outline-none focus:border-[#0f3e68]">
                                    </div>
                                </div>
                                <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                                    <div>
                                        <label class="block text-xs font-bold text-slate-700 mb-1">Danh mục cần báo giá *</label>
                                        <select id="quote-category" class="w-full px-3 py-2 text-xs sm:text-sm border border-slate-300 rounded focus:outline-none focus:border-[#0f3e68] bg-white">
                                            <option value="Trọn gói VLXD & Nội thất">Trọn gói VLXD & Nội thất công trình</option>
                                            <option value="Sơn nước & Chống thấm">Sơn (Jotun, Dulux, Tito, Chống thấm)</option>
                                            <option value="Thiết bị vệ sinh">Thiết bị vệ sinh (Bồn cầu, Sen vòi, Lavabo)</option>
                                            <option value="Gạch men ốp lát">Gạch men (Đồng Tâm, Kimgres)</option>
                                            <option value="Ngói lợp">Ngói lợp (DIC, Ngói Đất Việt, Sunrise)</option>
                                            <option value="Bồn nước Inox & Nhựa">Bồn nước (Letton, Sơn Hà, Tân Á)</option>
                                            <option value="Bình nóng lạnh">Bình nóng lạnh (Ariston, Ferroli)</option>
                                            <option value="Keo dán gạch, chà ron">Keo dán gạch, chà ron (Bestmix, Sika, Cá sấu)</option>
                                        </select>
                                    </div>
                                    <div>
                                        <label class="block text-xs font-bold text-slate-700 mb-1">Địa chỉ giao hàng / Công trình</label>
                                        <input id="quote-address" type="text" placeholder="Quận/Huyện, Đà Nẵng..." class="w-full px-3 py-2 text-xs sm:text-sm border border-slate-300 rounded focus:outline-none focus:border-[#0f3e68]">
                                    </div>
                                </div>
                                <div>
                                    <label class="block text-xs font-bold text-slate-700 mb-1">Nội dung chi tiết mã sản phẩm hoặc số lượng cần báo giá</label>
                                    <textarea id="quote-note" rows="3" placeholder="Nhập tên sản phẩm, mã hàng hoặc khối lượng dự kiến..." class="w-full px-3 py-2 text-xs sm:text-sm border border-slate-300 rounded focus:outline-none focus:border-[#0f3e68]"></textarea>
                                </div>
                                <div class="flex flex-wrap items-center gap-3 pt-1">
                                    <button type="submit" class="bg-[#0f3e68] hover:bg-[#1a568e] text-white font-bold text-xs sm:text-sm px-5 py-2.5 rounded shadow transition">
                                        <i class="fa-solid fa-paper-plane mr-1.5"></i>GỬI YÊU CẦU BÁO GIÁ
                                    </button>
                                    <a href="https://zalo.me/0932555605" target="_blank" rel="noopener" class="bg-amber-500 hover:bg-amber-600 text-white font-bold text-xs sm:text-sm px-4 py-2.5 rounded shadow transition">
                                        <i class="fa-solid fa-comments mr-1.5"></i>NHẬN BÁO GIÁ QUA ZALO: 0932.555.605
                                    </a>
                                </div>
                                <div id="quote-feedback" class="hidden p-3 rounded bg-emerald-50 border border-emerald-300 text-emerald-800 text-xs font-semibold"></div>
                            </form>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- SECTION 6: DANH MỤC CÁC BÀI VIẾT TRANG CHỦ (TIN TỨC & CẨM NANG) -->
        <section id="tin-tuc" class="section-blog-posts">
            <div class="flatsome-container">
                <div class="section-cat-header">
                    <h2 class="section-cat-title">
                        <i class="fa-solid fa-newspaper"></i>DANH MỤC BÀI VIẾT & TIN TỨC TRANG CHỦ
                    </h2>
                    <div class="subcat-pills">
                        <span class="subcat-pill">Kinh nghiệm chọn VLXD</span>
                        <span class="subcat-pill">Báo giá mới nhất</span>
                    </div>
                </div>

                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4">
                    <!-- Bài viết 1 -->
                    <article class="bg-white rounded-lg border border-slate-200 overflow-hidden shadow-sm flex flex-col justify-between">
                        <div>
                            <img src="https://drive.google.com/thumbnail?id=1DaeFx6AXIb9EdOjTVr2EcVqQD7k-q1Ns&sz=w600"
                                 onerror="this.onerror=null;this.src='https://placehold.co/500x320/0f3e68/ffffff?text=Showroom+Mai+Bao+Chau';"
                                 alt="Giới thiệu Công Ty TNHH Mai Bảo Châu"
                                 class="w-full h-40 object-cover">
                            <div class="p-3.5 space-y-2">
                                <h3 class="text-sm font-bold text-[#0f3e68] leading-snug">
                                    Giới thiệu CÔNG TY TNHH MAI BẢO CHÂU – Đại lý Thiết Bị Vệ Sinh & Gạch Men uy tín tại Đà Nẵng
                                </h3>
                                <p class="text-xs text-slate-600 leading-relaxed">
                                    Showroom Minh Huy (minhhuy.com) tại 199 Xô Viết Nghệ Tĩnh, Cẩm Lệ chuyên cung cấp thiết bị vệ sinh Inax, Viglacera và gạch men Đồng Tâm chính hãng...
                                </p>
                            </div>
                        </div>
                        <div class="px-3.5 pb-3 pt-1 border-t border-slate-100 flex items-center justify-between text-[11px] text-slate-500">
                            <span><i class="fa-regular fa-calendar mr-1"></i>Cẩm nang VLXD</span>
                            <a href="#form-bao-gia" class="font-bold text-[#0f3e68] hover:underline">Nhận tư vấn &rarr;</a>
                        </div>
                    </article>

                    <!-- Bài viết 2 -->
                    <article class="bg-white rounded-lg border border-slate-200 overflow-hidden shadow-sm flex flex-col justify-between">
                        <div>
                            <img src="https://drive.google.com/thumbnail?id=1X31hmhpLVVORV-tmMSZYzBO-qtpyusry&sz=w600"
                                 onerror="this.onerror=null;this.src='https://placehold.co/500x320/1e5b94/ffffff?text=Son+Jotun+Dulux';"
                                 alt="Đại lý Sơn Jotun Dulux tại Đà Nẵng"
                                 class="w-full h-40 object-cover">
                            <div class="p-3.5 space-y-2">
                                <h3 class="text-sm font-bold text-[#0f3e68] leading-snug">
                                    Kinh nghiệm chọn Sơn ngoại thất & Chống thấm Sika, Jotun, Dulux bền màu cho khí hậu miền Trung
                                </h3>
                                <p class="text-xs text-slate-600 leading-relaxed">
                                    Hướng dẫn quy trình thi công sơn lót chống kiềm, sơn phủ Jotashield và chất chống thấm Sika, Bestmix giúp bảo vệ tường nhà tối đa...
                                </p>
                            </div>
                        </div>
                        <div class="px-3.5 pb-3 pt-1 border-t border-slate-100 flex items-center justify-between text-[11px] text-slate-500">
                            <span><i class="fa-regular fa-calendar mr-1"></i>Tư vấn Sơn nước</span>
                            <a href="#cat-son" class="font-bold text-[#0f3e68] hover:underline">Xem sản phẩm &rarr;</a>
                        </div>
                    </article>

                    <!-- Bài viết 3 -->
                    <article class="bg-white rounded-lg border border-slate-200 overflow-hidden shadow-sm flex flex-col justify-between">
                        <div>
                            <img src="https://drive.google.com/thumbnail?id=171kMlCqYFeFpvYcgH1wQbaIMszY0Ns3O&sz=w600"
                                 onerror="this.onerror=null;this.src='https://placehold.co/500x320/0f3e68/ffffff?text=Gach+Men+Dong+Tam';"
                                 alt="Kinh doanh gạch men Đồng Tâm Kimgres"
                                 class="w-full h-40 object-cover">
                            <div class="p-3.5 space-y-2">
                                <h3 class="text-sm font-bold text-[#0f3e68] leading-snug">
                                    Cách phối Gạch men Porcelain 80x80, 60x60 Đồng Tâm & Kimgres sang trọng cho phòng khách
                                </h3>
                                <p class="text-xs text-slate-600 leading-relaxed">
                                    Tổng hợp các mẫu gạch Porcelain kháng khuẩn, gạch 2 da bóng kính và keo dán gạch, keo chà ron chống thấm ố màu tốt nhất hiện nay...
                                </p>
                            </div>
                        </div>
                        <div class="px-3.5 pb-3 pt-1 border-t border-slate-100 flex items-center justify-between text-[11px] text-slate-500">
                            <span><i class="fa-regular fa-calendar mr-1"></i>Xu hướng Nội thất</span>
                            <a href="#cat-gach-men" class="font-bold text-[#0f3e68] hover:underline">Xem mẫu gạch &rarr;</a>
                        </div>
                    </article>

                    <!-- Bài viết 4 -->
                    <article class="bg-white rounded-lg border border-slate-200 overflow-hidden shadow-sm flex flex-col justify-between">
                        <div>
                            <img src="https://drive.google.com/thumbnail?id=1t8U7WQsmDbGWzmSelkxzjVv8M0BvIxAg&sz=w600"
                                 onerror="this.onerror=null;this.src='https://placehold.co/500x320/1e5b94/ffffff?text=Bon+Nuoc+Binh+Nong+Lanh';"
                                 alt="Bồn nước và Bình nóng lạnh Ariston Ferroli"
                                 class="w-full h-40 object-cover">
                            <div class="p-3.5 space-y-2">
                                <h3 class="text-sm font-bold text-[#0f3e68] leading-snug">
                                    Tư vấn chọn dung tích Bồn nước Tân Á, Sơn Hà & Bình nóng lạnh Ariston, Ferroli tiết kiệm điện
                                </h3>
                                <p class="text-xs text-slate-600 leading-relaxed">
                                    Giải pháp chọn bồn nước Inox 304 đứng/ngang và máy nước nóng gián tiếp, trực tiếp an toàn cho gia đình từ 4 đến 8 thành viên...
                                </p>
                            </div>
                        </div>
                        <div class="px-3.5 pb-3 pt-1 border-t border-slate-100 flex items-center justify-between text-[11px] text-slate-500">
                            <span><i class="fa-regular fa-calendar mr-1"></i>Thiết bị phòng tắm</span>
                            <a href="#cat-binh-nong-lanh" class="font-bold text-[#0f3e68] hover:underline">Xem chi tiết &rarr;</a>
                        </div>
                    </article>
                </div>
            </div>
        </section>

        <!-- SECTION 7: DANH MỤC CÁC ĐỐI TÁC THƯƠNG HIỆU -->
        <section id="doi-tac" class="section-partners">
            <div class="flatsome-container">
                <div class="bg-white rounded-lg border border-slate-200 p-4 shadow-sm">
                    <div class="flex items-center justify-between mb-3 pb-2 border-b border-slate-100">
                        <h2 class="text-xs sm:text-sm font-extrabold text-[#0f3e68] uppercase">
                            <i class="fa-solid fa-handshake text-amber-600 mr-1.5"></i>ĐỐI TÁC & THƯƠNG HIỆU PHÂN PHỐI CHÍNH HÃNG
                        </h2>
                        <span class="text-[11px] text-slate-500">100% Sản phẩm chính hãng tại minhhuy.com</span>
                    </div>
                    <div class="grid grid-cols-3 sm:grid-cols-4 md:grid-cols-7 gap-2.5 text-center">
                        <div class="p-2.5 rounded border border-slate-200 bg-slate-50 font-extrabold text-xs text-[#0f3e68]">JOTUN</div>
                        <div class="p-2.5 rounded border border-slate-200 bg-slate-50 font-extrabold text-xs text-[#0f3e68]">DULUX - MAXILITE</div>
                        <div class="p-2.5 rounded border border-slate-200 bg-slate-50 font-extrabold text-xs text-[#0f3e68]">INAX</div>
                        <div class="p-2.5 rounded border border-slate-200 bg-slate-50 font-extrabold text-xs text-[#0f3e68]">VIGLACERA</div>
                        <div class="p-2.5 rounded border border-slate-200 bg-slate-50 font-extrabold text-xs text-[#0f3e68]">ĐỒNG TÂM</div>
                        <div class="p-2.5 rounded border border-slate-200 bg-slate-50 font-extrabold text-xs text-[#0f3e68]">KIMGRES</div>
                        <div class="p-2.5 rounded border border-slate-200 bg-slate-50 font-extrabold text-xs text-[#0f3e68]">ARISTON</div>
                        <div class="p-2.5 rounded border border-slate-200 bg-slate-50 font-extrabold text-xs text-[#0f3e68]">FERROLI</div>
                        <div class="p-2.5 rounded border border-slate-200 bg-slate-50 font-extrabold text-xs text-[#0f3e68]">TÂN Á ĐẠI THÀNH</div>
                        <div class="p-2.5 rounded border border-slate-200 bg-slate-50 font-extrabold text-xs text-[#0f3e68]">SƠN HÀ</div>
                        <div class="p-2.5 rounded border border-slate-200 bg-slate-50 font-extrabold text-xs text-[#0f3e68]">SIKA</div>
                        <div class="p-2.5 rounded border border-slate-200 bg-slate-50 font-extrabold text-xs text-[#0f3e68]">BESTMIX</div>
                        <div class="p-2.5 rounded border border-slate-200 bg-slate-50 font-extrabold text-xs text-[#0f3e68]">NGÓI ĐẤT VIỆT</div>
                        <div class="p-2.5 rounded border border-slate-200 bg-slate-50 font-extrabold text-xs text-[#0f3e68]">NGÓI DIC</div>
                    </div>
                </div>
            </div>
        </section>

        <!-- SECTION 8: ĐƯA GOOGLE MAP VÀ FANPAGE FACEBOOK RA NGOÀI TRANG CHỦ -->
        <section id="lien-he-bando" class="section-map-fanpage">
            <div class="flatsome-container">
                <div class="grid grid-cols-1 lg:grid-cols-12 gap-5">

                    <!-- Cột Google Map ngoài trang chủ (7/12) -->
                    <div class="lg:col-span-7 bg-white rounded-lg border border-slate-200 p-4 shadow-sm flex flex-col justify-between space-y-3">
                        <div class="flex flex-wrap items-center justify-between gap-2 border-b border-slate-100 pb-2.5">
                            <div>
                                <h2 class="text-sm sm:text-base font-extrabold text-[#0f3e68] uppercase">
                                    <i class="fa-solid fa-map-location-dot text-red-600 mr-1.5"></i>BẢN ĐỒ ĐƯỜNG ĐI ĐẾN CỬA HÀNG MINH HUY
                                </h2>
                                <p class="text-xs text-slate-600 mt-0.5">
                                    Địa chỉ: <strong>199 Xô Viết Nghệ Tĩnh, Quận Cẩm Lệ, TP. Đà Nẵng</strong> — ĐT: <strong>0932.555.605</strong>
                                </p>
                            </div>
                            <a href="https://share.google/LUMi7g7OSirIMX58u" target="_blank" rel="noopener" class="inline-flex items-center gap-1.5 bg-[#0f3e68] hover:bg-[#1a568e] text-white text-xs font-bold px-3 py-1.5 rounded transition">
                                <i class="fa-solid fa-diamond-turn-right"></i>Mở Google Maps
                            </a>
                        </div>

                        <!-- Nhúng bản đồ Google Map thực tế tại 199 Xô Viết Nghệ Tĩnh, Cẩm Lệ, Đà Nẵng -->
                        <div class="w-full h-72 sm:h-80 rounded-lg overflow-hidden border border-slate-200 relative bg-slate-100">
                            <iframe
                                title="Bản đồ Công Ty TNHH Mai Bảo Châu - 199 Xô Viết Nghệ Tĩnh, Cẩm Lệ, Đà Nẵng"
                                src="https://maps.google.com/maps?q=199%20X%C3%B4%20Vi%E1%BA%BFt%20Ngh%E1%BB%87%20T%C4%A9nh,%20C%E1%BA%A9m%20L%E1%BB%87,%20%C4%90%C3%A0%20N%E1%BA%B5ng&t=&z=16&ie=UTF8&iwloc=&output=embed"
                                class="w-full h-full border-0"
                                loading="lazy"
                                referrerpolicy="no-referrer-when-downgrade">
                            </iframe>
                        </div>

                        <div class="flex flex-wrap items-center justify-between gap-2 text-xs bg-slate-50 p-2.5 rounded border border-slate-200">
                            <span><i class="fa-solid fa-location-crosshairs text-[#0f3e68] mr-1"></i>Cửa Hàng Gạch Men - Thiết Bị Vệ Sinh Minh Huy (Công Ty TNHH Mai Bảo Châu)</span>
                            <a href="https://share.google/LUMi7g7OSirIMX58u" target="_blank" rel="noopener" class="font-bold text-red-600 hover:underline">
                                Xem vị trí trên Google Map &rarr;
                            </a>
                        </div>
                    </div>

                    <!-- Cột Fanpage Facebook ngoài trang chủ (5/12) -->
                    <div class="lg:col-span-5 bg-white rounded-lg border border-slate-200 p-4 shadow-sm flex flex-col justify-between space-y-3">
                        <div class="flex items-center justify-between border-b border-slate-100 pb-2.5">
                            <div>
                                <h2 class="text-sm sm:text-base font-extrabold text-[#0f3e68] uppercase">
                                    <i class="fa-brands fa-facebook text-[#1877F2] mr-1.5"></i>FANPAGE FACEBOOK CHÍNH THỨC
                                </h2>
                                <p class="text-xs text-slate-600 mt-0.5">Kết nối & xem mẫu hàng mới về mỗi ngày</p>
                            </div>
                            <a href="https://www.facebook.com/profile.php?id=100054322668588" target="_blank" rel="noopener" class="bg-[#1877F2] hover:bg-blue-700 text-white text-xs font-bold px-3 py-1.5 rounded transition">
                                <i class="fa-solid fa-thumbs-up mr-1"></i>Theo dõi
                            </a>
                        </div>

                        <!-- Khung hiển thị trực quan Fanpage + Plugin Facebook -->
                        <div class="rounded-lg border border-slate-200 overflow-hidden bg-slate-50">
                            <div class="relative h-32 bg-gradient-to-r from-[#0f3e68] to-[#1e5b94] p-3 flex items-end">
                                <img src="https://drive.google.com/thumbnail?id=1DaeFx6AXIb9EdOjTVr2EcVqQD7k-q1Ns&sz=w600"
                                     onerror="this.onerror=null;this.src='https://placehold.co/600x200/0f3e68/ffffff?text=Fanpage+Mai+Bao+Chau';"
                                     alt="Fanpage Công Ty TNHH Mai Bảo Châu"
                                     class="absolute inset-0 w-full h-full object-cover opacity-35">
                                <div class="relative z-10 flex items-center gap-3 text-white">
                                    <div class="w-12 h-12 rounded-full bg-white text-[#0f3e68] font-extrabold flex items-center justify-center border-2 border-amber-400 shadow">
                                        MBC
                                    </div>
                                    <div>
                                        <div class="font-extrabold text-sm leading-tight">CÔNG TY TNHH MAI BẢO CHÂU</div>
                                        <div class="text-[11px] text-amber-300">Showroom VLXD & Nội Thất Minh Huy • 0932.555.605</div>
                                    </div>
                                </div>
                            </div>
                            <div class="p-3 space-y-2 text-xs text-slate-700">
                                <p><i class="fa-solid fa-check text-emerald-600 mr-1.5"></i>Cập nhật mẫu Gạch men, Thiết bị vệ sinh, Sơn nước, Bồn nước, Bình nóng lạnh mới nhất.</p>
                                <p><i class="fa-solid fa-location-dot text-red-600 mr-1.5"></i>Địa chỉ: 199 Xô Viết Nghệ Tĩnh, Cẩm Lệ, Đà Nẵng</p>
                                <div class="w-full overflow-hidden rounded border border-slate-200 bg-white pt-1">
                                    <iframe
                                        title="Fanpage Facebook Công Ty TNHH Mai Bảo Châu"
                                        src="https://www.facebook.com/plugins/page.php?href=https%3A%2F%2Fwww.facebook.com%2Fprofile.php%3Fid%3D100054322668588&tabs=timeline&width=340&height=180&small_header=true&adapt_container_width=true&hide_cover=false&show_facepile=true"
                                        width="100%"
                                        height="160"
                                        style="border:none;overflow:hidden"
                                        scrolling="no"
                                        frameborder="0"
                                        allowfullscreen="true"
                                        allow="autoplay; clipboard-write; encrypted-media; picture-in-picture; web-share">
                                    </iframe>
                                </div>
                            </div>
                        </div>

                        <div class="grid grid-cols-2 gap-2 text-xs font-bold">
                            <a href="https://www.facebook.com/profile.php?id=100054322668588" target="_blank" rel="noopener" class="py-2 px-3 rounded bg-[#1877F2] text-white text-center hover:bg-blue-700 transition">
                                <i class="fa-brands fa-facebook-f mr-1"></i>Mở Fanpage Facebook
                            </a>
                            <a href="https://zalo.me/0932555605" target="_blank" rel="noopener" class="py-2 px-3 rounded bg-[#0068ff] text-white text-center hover:bg-blue-600 transition">
                                <i class="fa-solid fa-comment-dots mr-1"></i>Nhắn Tin Zalo
                            </a>
                        </div>
                    </div>

                </div>
            </div>
        </section>

    </main>

    <!-- ==========================================
         FOOTER FLATSOME (#footer)
    =========================================== -->
    <footer id="footer" class="bg-[#0a2c4d] text-slate-200 pt-8 pb-20 lg:pb-8 mt-8 border-t-4 border-amber-500">
        <div class="flatsome-container">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 pb-6 border-b border-white/10 text-xs sm:text-sm">

                <!-- Cột 1: Thông tin công ty -->
                <div class="space-y-2.5">
                    <h3 class="text-white font-extrabold text-sm sm:text-base uppercase">CÔNG TY TNHH MAI BẢO CHÂU</h3>
                    <div class="text-amber-300 font-bold text-xs">SHOWROOM VLXD & NỘI THẤT MINH HUY (MINHHUY.COM)</div>
                    <p class="text-xs text-slate-300 leading-relaxed">
                        Chuyên phân phối Sơn Jotun, Dulux, Thiết bị vệ sinh INAX, Viglacera, Gạch men Đồng Tâm, Kimgres, Ngói lợp, Bồn nước, Bình nóng lạnh, Keo dán gạch chính hãng tại Đà Nẵng.
                    </p>
                    <ul class="space-y-1.5 text-xs">
                        <li><i class="fa-solid fa-location-dot text-amber-400 mr-2"></i><strong>Địa chỉ:</strong> 199 Xô Viết Nghệ Tĩnh, Cẩm Lệ, Đà Nẵng</li>
                        <li><i class="fa-solid fa-phone-volume text-amber-400 mr-2"></i><strong>Điện thoại / Zalo:</strong> <a href="tel:0932555605" class="text-amber-300 font-bold">0932.555.605</a></li>
                        <li><i class="fa-solid fa-globe text-amber-400 mr-2"></i><strong>Website:</strong> minhhuy.com</li>
                    </ul>
                </div>

                <!-- Cột 2: Danh mục sản phẩm -->
                <div class="space-y-2">
                    <h3 class="text-white font-extrabold text-sm uppercase">DANH MỤC SẢN PHẨM</h3>
                    <ul class="space-y-1.5 text-xs">
                        <li><a href="#cat-son" class="hover:text-amber-300 transition">&rsaquo; Sơn Jotun, Dulux - Maxilite, Tito, Chống thấm</a></li>
                        <li><a href="#cat-tbvs" class="hover:text-amber-300 transition">&rsaquo; Thiết bị vệ sinh: Bồn cầu, Sen vòi, Lavabo, Gương</a></li>
                        <li><a href="#cat-gach-men" class="hover:text-amber-300 transition">&rsaquo; Gạch men: Đồng Tâm (80x80, 60x60, 30x60), Kimgres</a></li>
                        <li><a href="#cat-ngoi-lop" class="hover:text-amber-300 transition">&rsaquo; Ngói lợp: DIC, Ngói Đất Việt, Ngói màu Sunrise</a></li>
                        <li><a href="#cat-bon-nuoc" class="hover:text-amber-300 transition">&rsaquo; Bồn nước: Letton, Sơn Hà, Tân Á Đại Thành</a></li>
                        <li><a href="#cat-binh-nong-lanh" class="hover:text-amber-300 transition">&rsaquo; Bình nóng lạnh: Ariston, Ferroli</a></li>
                        <li><a href="#cat-keo-dan-gach" class="hover:text-amber-300 transition">&rsaquo; Keo dán gạch, chà ron: Bestmix, Đồng Tâm, Sika</a></li>
                    </ul>
                </div>

                <!-- Cột 3: Hỗ trợ khách hàng -->
                <div class="space-y-2">
                    <h3 class="text-white font-extrabold text-sm uppercase">CHÍNH SÁCH & HỖ TRỢ</h3>
                    <ul class="space-y-1.5 text-xs">
                        <li><a href="#form-bao-gia" class="hover:text-amber-300 transition">&rsaquo; Yêu cầu báo giá sỉ công trình</a></li>
                        <li><a href="#anh-thuc-te" class="hover:text-amber-300 transition">&rsaquo; Hình ảnh thực tế tại cửa hàng</a></li>
                        <li><a href="#doi-tac" class="hover:text-amber-300 transition">&rsaquo; Hệ thống đối tác thương hiệu</a></li>
                        <li><a href="#tin-tuc" class="hover:text-amber-300 transition">&rsaquo; Tin tức & Cẩm nang xây dựng</a></li>
                        <li><a href="https://share.google/LUMi7g7OSirIMX58u" target="_blank" rel="noopener" class="hover:text-amber-300 transition">&rsaquo; Chỉ đường Google Maps</a></li>
                        <li><a href="https://www.facebook.com/profile.php?id=100054322668588" target="_blank" rel="noopener" class="hover:text-amber-300 transition">&rsaquo; Kết nối Fanpage Facebook</a></li>
                    </ul>
                </div>

                <!-- Cột 4: Liên kết nhanh -->
                <div class="space-y-2.5">
                    <h3 class="text-white font-extrabold text-sm uppercase">LIÊN HỆ NHANH</h3>
                    <p class="text-xs text-slate-300">Gọi ngay hoặc nhắn Zalo để nhận bảng giá chiết khấu tốt nhất hôm nay:</p>
                    <div class="space-y-2 pt-1">
                        <a href="tel:0932555605" class="flex items-center justify-center gap-2 w-full py-2 px-3 rounded bg-red-600 hover:bg-red-700 text-white font-bold text-xs transition">
                            <i class="fa-solid fa-phone-volume"></i>HOTLINE: 0932.555.605
                        </a>
                        <a href="https://zalo.me/0932555605" target="_blank" rel="noopener" class="flex items-center justify-center gap-2 w-full py-2 px-3 rounded bg-[#0068ff] hover:bg-blue-600 text-white font-bold text-xs transition">
                            <i class="fa-solid fa-comments"></i>CHAT ZALO: 0932.555.605
                        </a>
                        <a href="https://www.facebook.com/profile.php?id=100054322668588" target="_blank" rel="noopener" class="flex items-center justify-center gap-2 w-full py-2 px-3 rounded bg-[#1877F2] hover:bg-blue-700 text-white font-bold text-xs transition">
                            <i class="fa-brands fa-facebook"></i>FANPAGE MAI BẢO CHÂU
                        </a>
                    </div>
                </div>

            </div>

            <div class="pt-4 text-center text-xs text-slate-400">
                Copyright 2026 &copy; <strong>CÔNG TY TNHH MAI BẢO CHÂU (minhhuy.com)</strong> – Địa chỉ: 199 Xô Viết Nghệ Tĩnh, Cẩm Lệ, Đà Nẵng | ĐT: 0932.555.605
            </div>
        </div>
    </footer>

    <!-- ==========================================
         CÁC NÚT LIÊN HỆ NỔI BẬT (ZALO, FACEBOOK, HOTLINE)
         Tương thích hoàn hảo trên cả máy tính và điện thoại
    =========================================== -->
    <div class="fixed right-3 bottom-4 z-50 flex flex-col items-end gap-2.5">
        <!-- Nút Facebook Fanpage -->
        <a href="https://www.facebook.com/profile.php?id=100054322668588" target="_blank" rel="noopener"
           class="flex items-center gap-2 bg-[#1877F2] hover:bg-blue-700 text-white px-3 py-2 rounded-full shadow-lg transition">
            <i class="fa-brands fa-facebook-f text-sm w-4 text-center"></i>
            <span class="text-xs font-bold">Fanpage</span>
        </a>

        <!-- Nút Chat Zalo -->
        <a href="https://zalo.me/0932555605" target="_blank" rel="noopener"
           class="flex items-center gap-2 bg-[#0068ff] hover:bg-blue-600 text-white px-3 py-2 rounded-full shadow-lg transition">
            <i class="fa-solid fa-comment-dots text-sm w-4 text-center"></i>
            <span class="text-xs font-bold">Zalo: 0932.555.605</span>
        </a>

        <!-- Nút Gọi Hotline nổi bật -->
        <a href="tel:0932555605"
           class="floating-btn-pulse flex items-center gap-2 bg-red-600 hover:bg-red-700 text-white px-3.5 py-2.5 rounded-full shadow-xl transition">
            <i class="fa-solid fa-phone-volume text-sm"></i>
            <span class="text-xs font-extrabold">0932.555.605</span>
        </a>
    </div>

    <!-- ==========================================
         JAVASCRIPT XỬ LÝ DỮ LIỆU SẢN PHẨM & TƯƠNG TÁC
    =========================================== -->
    <script>
        /* Danh sách đầy đủ 19 file ảnh sản phẩm thực tế từ Google Drive của khách hàng */
        const driveProductFiles = [
            { id: "1P2fePSvPXm6YIcNDixVa0YwFWshcHFDY", name: "Bồn cầu liền khối men sứ chống bám bẩn cao cấp tại Showroom Minh Huy", cat: "Thiết bị vệ sinh", oldPrice: "4.650.000₫", newPrice: "3.720.000₫", discount: "-20%" },
            { id: "11z7ir7cmqEcdrYuAThZvpOhgUVFsLUnP", name: "Bộ sen cây tắm đứng nóng lạnh Inax / Viglacera chính hãng", cat: "Thiết bị vệ sinh", oldPrice: "3.450.000₫", newPrice: "2.790.000₫", discount: "-19%" },
            { id: "1KTDzdSGqiXWuLZDkPoDD7oZZVL-5F3Rr", name: "Chậu rửa mặt Lavabo đặt bàn & Tủ chậu phòng tắm sang trọng", cat: "Thiết bị vệ sinh", oldPrice: "2.800.000₫", newPrice: "2.290.000₫", discount: "-18%" },
            { id: "1X31hmhpLVVORV-tmMSZYzBO-qtpyusry", name: "Sơn ngoại thất Jotun Jotashield & Dulux bền màu chống thấm tối ưu", cat: "Sơn nước", oldPrice: "2.350.000₫", newPrice: "1.950.000₫", discount: "-17%" },
            { id: "171kMlCqYFeFpvYcgH1wQbaIMszY0Ns3O", name: "Gạch men Porcelain bóng kiếng 80x80 vân đá tự nhiên Đồng Tâm", cat: "Gạch men", oldPrice: "340.000₫/m²", newPrice: "279.000₫/m²", discount: "-18%" },
            { id: "1t8U7WQsmDbGWzmSelkxzjVv8M0BvIxAg", name: "Bình nóng lạnh gián tiếp Ariston / Ferroli tiết kiệm điện năng", cat: "Bình nóng lạnh", oldPrice: "3.650.000₫", newPrice: "2.990.000₫", discount: "-18%" },
            { id: "1uqL6ACCB5ne0G1BYkXCurdnrsf1m2lr4", name: "Bồn cầu 2 khối Viglacera / Inax xả xoáy siêu sạch tiết kiệm nước", cat: "Thiết bị vệ sinh", oldPrice: "2.650.000₫", newPrice: "2.150.000₫", discount: "-19%" },
            { id: "1NwR4v0eypEtIwPi6NJVJCKoNCFFQ8G54", name: "Sen tắm nóng lạnh & Vòi lavabo Inox 304 mạ Crom sáng bóng", cat: "Thiết bị vệ sinh", oldPrice: "1.850.000₫", newPrice: "1.480.000₫", discount: "-20%" },
            { id: "19jauCH_X7lcc0KNlu2OJ75CRiw3ArT7r", name: "Gương soi phòng tắm tráng bạc chống ố mốc & Kệ gương", cat: "Thiết bị vệ sinh", oldPrice: "980.000₫", newPrice: "790.000₫", discount: "-19%" },
            { id: "1_HXfxWiPLtWiayxMPjgFCsl1WS1wGb7h", name: "Gạch lát nền 60x60 Kimgres & Đồng Tâm chống trầy xước", cat: "Gạch men", oldPrice: "265.000₫/m²", newPrice: "219.000₫/m²", discount: "-17%" },
            { id: "1ciwHcFfmGbsIyjTsi9KlyIsx6EXBNJTN", name: "Gạch ốp tường 30x60 vân đá phòng tắm & phòng bếp hiện đại", cat: "Gạch men", oldPrice: "240.000₫/m²", newPrice: "195.000₫/m²", discount: "-19%" },
            { id: "1vHG-pgeryaSItJoQ5ciiCGSWA7SJSU8c", name: "Ngói lợp màu cao cấp DIC / Ngói Đất Việt bền màu chống rêu mốc", cat: "Ngói lợp", oldPrice: "22.000₫/viên", newPrice: "18.500₫/viên", discount: "-16%" },
            { id: "1X-ECML9CKN4ycBfVFu4pC0wnqzTS12CP", name: "Bồn nước Inox đứng & ngang Tân Á Đại Thành / Sơn Hà chính hãng", cat: "Bồn nước", oldPrice: "4.200.000₫", newPrice: "3.490.000₫", discount: "-17%" },
            { id: "1CGBZ4cuB7DMWadnoktlMoji6MB3dioC-", name: "Sơn nội thất Jotun Essence dễ lau chùi & Sơn trắng trần chuyên dụng", cat: "Sơn nước", oldPrice: "1.650.000₫", newPrice: "1.350.000₫", discount: "-18%" },
            { id: "17YrxXteZmzhvVRYgfaklNGC2hKjN09N8", name: "Hợp chất chống thấm Sika / Bestmix chuyên dụng sàn mái & nhà vệ sinh", cat: "Sơn nước", oldPrice: "890.000₫", newPrice: "730.000₫", discount: "-18%" },
            { id: "19k5uWHn_xeas2_BMP_JgBDwwu-IysSRP", name: "Bộ phụ kiện phòng tắm 6 món Inox 304 & Vắt khăn giàn cao cấp", cat: "Thiết bị vệ sinh", oldPrice: "1.450.000₫", newPrice: "1.160.000₫", discount: "-20%" },
            { id: "1oah4j6YAPIsJacMYQFJ0JGVemrMwqCgf", name: "Máy nước nóng trực tiếp Ariston / Ferroli chống giật ELCB an toàn", cat: "Bình nóng lạnh", oldPrice: "2.950.000₫", newPrice: "2.390.000₫", discount: "-19%" },
            { id: "15IWAPhzVLsyUO5TDRoWXxvncrHoFcH1_", name: "Keo dán gạch & Keo chà ron Sika / Bestmix / Cá Sấu bám dính siêu cường", cat: "Keo dán gạch", oldPrice: "320.000₫/bao", newPrice: "265.000₫/bao", discount: "-17%" },
            { id: "1WLKyUBxRc63xFN9GBUhFcqE0xPo0sQKh", name: "Chậu rửa chén bát Inox 304 đúc nguyên khối & Vòi rửa nóng lạnh", cat: "Thiết bị vệ sinh", oldPrice: "2.750.000₫", newPrice: "2.190.000₫", discount: "-20%" }
        ];

        /* 7 Danh mục sản phẩm chuẩn web mẫu noithatngonguyen.com */
        const sampleWebsiteCategories = [
            {
                id: "cat-son",
                title: "SƠN",
                icon: "fa-fill-drip",
                subcategories: ["Jotun", "Dulux-maxilite", "Tito", "Chống thấm Sika - Bestmix - Mapei"],
                products: [
                    { name: "Essence Sơn Trắng Trần Chuyên Dụng", driveId: "1CGBZ4cuB7DMWadnoktlMoji6MB3dioC-", oldPrice: "1.250.000₫", newPrice: "1.020.000₫", discount: "-18%" },
                    { name: "Essence Che phủ tối đa mờ", driveId: "1X31hmhpLVVORV-tmMSZYzBO-qtpyusry", oldPrice: "1.580.000₫", newPrice: "1.290.000₫", discount: "-18%" },
                    { name: "Essence Che Phủ Tối Đa Bóng", driveId: "1CGBZ4cuB7DMWadnoktlMoji6MB3dioC-", oldPrice: "1.690.000₫", newPrice: "1.380.000₫", discount: "-18%" },
                    { name: "Sơn ngoại thất Toughshield Max", driveId: "1X31hmhpLVVORV-tmMSZYzBO-qtpyusry", oldPrice: "1.950.000₫", newPrice: "1.590.000₫", discount: "-18%" },
                    { name: "Sơn ngoại thất Jotun Tough Shield", driveId: "17YrxXteZmzhvVRYgfaklNGC2hKjN09N8", oldPrice: "1.750.000₫", newPrice: "1.420.000₫", discount: "-19%" },
                    { name: "Sơn Jotashield Sạch Vượt Trội", driveId: "1X31hmhpLVVORV-tmMSZYzBO-qtpyusry", oldPrice: "2.480.000₫", newPrice: "1.990.000₫", discount: "-20%" },
                    { name: "Jotun Jotashield che phủ vết nứt", driveId: "1CGBZ4cuB7DMWadnoktlMoji6MB3dioC-", oldPrice: "2.750.000₫", newPrice: "2.250.000₫", discount: "-18%" },
                    { name: "Jotun Jotashield Bền Màu Toàn Diện", driveId: "17YrxXteZmzhvVRYgfaklNGC2hKjN09N8", oldPrice: "2.890.000₫", newPrice: "2.350.000₫", discount: "-19%" }
                ]
            },
            {
                id: "cat-tbvs",
                title: "THIẾT BỊ VỆ SINH",
                icon: "fa-shower",
                subcategories: ["Bồn cầu", "Sen vòi", "Lavabo", "Gương", "Phụ kiện nhà tắm"],
                products: [
                    { name: "Sen tắm âm tường Inax BFV-81SEHW", driveId: "11z7ir7cmqEcdrYuAThZvpOhgUVFsLUnP", oldPrice: "6.450.000₫", newPrice: "5.160.000₫", discount: "-20%" },
                    { name: "Sen cây Viglacera VG519", driveId: "1NwR4v0eypEtIwPi6NJVJCKoNCFFQ8G54", oldPrice: "3.550.000₫", newPrice: "2.850.000₫", discount: "-20%" },
                    { name: "Sen cây Viglacera VG540", driveId: "11z7ir7cmqEcdrYuAThZvpOhgUVFsLUnP", oldPrice: "3.850.000₫", newPrice: "3.120.000₫", discount: "-19%" },
                    { name: "Cây sen tắm Inax BFV – CL1", driveId: "1NwR4v0eypEtIwPi6NJVJCKoNCFFQ8G54", oldPrice: "4.650.000₫", newPrice: "3.790.000₫", discount: "-18%" },
                    { name: "Sen Cây Tắm Inax BFV-615S-8C Nóng Lạnh", driveId: "1P2fePSvPXm6YIcNDixVa0YwFWshcHFDY", oldPrice: "4.950.000₫", newPrice: "3.960.000₫", discount: "-20%" },
                    { name: "Bồn cầu 2 khối Viglacera VI6 nắp thường", driveId: "1uqL6ACCB5ne0G1BYkXCurdnrsf1m2lr4", oldPrice: "2.350.000₫", newPrice: "1.890.000₫", discount: "-20%" },
                    { name: "Bộ phụ kiện sen cây Caesar BS124", driveId: "19k5uWHn_xeas2_BMP_JgBDwwu-IysSRP", oldPrice: "1.450.000₫", newPrice: "1.180.000₫", discount: "-19%" },
                    { name: "Chậu Lavabo & Gương phòng tắm Inax", driveId: "1KTDzdSGqiXWuLZDkPoDD7oZZVL-5F3Rr", oldPrice: "2.400.000₫", newPrice: "1.950.000₫", discount: "-19%" }
                ]
            },
            {
                id: "cat-gach-men",
                title: "GẠCH MEN",
                icon: "fa-border-all",
                subcategories: ["Đồng Tâm 80x80", "Gạch 60x60", "Gạch 40x80", "Gạch 40x40", "Gạch 30x60", "Kimgres"],
                products: [
                    { name: "GẠCH PORCELAIN KHÁNG KHUẨN 8080FANSIPAN007-FP", driveId: "171kMlCqYFeFpvYcgH1wQbaIMszY0Ns3O", oldPrice: "365.000₫/m²", newPrice: "295.000₫/m²", discount: "-19%" },
                    { name: "GẠCH PORCELAIN 2 DA 8080PLATINUM003", driveId: "1_HXfxWiPLtWiayxMPjgFCsl1WS1wGb7h", oldPrice: "380.000₫/m²", newPrice: "310.000₫/m²", discount: "-18%" },
                    { name: "GẠCH PORCELAIN 2 DA 8080PLATINUM001", driveId: "1ciwHcFfmGbsIyjTsi9KlyIsx6EXBNJTN", oldPrice: "380.000₫/m²", newPrice: "310.000₫/m²", discount: "-18%" },
                    { name: "GẠCH PORCELAIN KHÁNG KHUẨN 8080DONGVAN010-FP-H+", driveId: "171kMlCqYFeFpvYcgH1wQbaIMszY0Ns3O", oldPrice: "350.000₫/m²", newPrice: "285.000₫/m²", discount: "-19%" },
                    { name: "GẠCH PORCELAIN KHÁNG KHUẨN 8080DONGVAN009-FP-H+", driveId: "1_HXfxWiPLtWiayxMPjgFCsl1WS1wGb7h", oldPrice: "350.000₫/m²", newPrice: "285.000₫/m²", discount: "-19%" },
                    { name: "GẠCH PORCELAIN KHÁNG KHUẨN 8080DONGVAN008-FP-H+", driveId: "1ciwHcFfmGbsIyjTsi9KlyIsx6EXBNJTN", oldPrice: "345.000₫/m²", newPrice: "279.000₫/m²", discount: "-19%" },
                    { name: "GẠCH PORCELAIN KHÁNG KHUẨN 8080DONGVAN006-FP-H+", driveId: "171kMlCqYFeFpvYcgH1wQbaIMszY0Ns3O", oldPrice: "345.000₫/m²", newPrice: "279.000₫/m²", discount: "-19%" },
                    { name: "GẠCH PORCELAIN KHÁNG KHUẨN 8080DONGVAN005-FP-H+", driveId: "1_HXfxWiPLtWiayxMPjgFCsl1WS1wGb7h", oldPrice: "345.000₫/m²", newPrice: "279.000₫/m²", discount: "-19%" }
                ]
            },
            {
                id: "cat-ngoi-lop",
                title: "NGÓI LỢP",
                icon: "fa-house-chimney",
                subcategories: ["DIC", "Ngói Đất Việt", "Ngói Màu Sunrise"],
                products: [
                    { name: "Ngói Lợp Đỏ tươi DT10S", driveId: "1vHG-pgeryaSItJoQ5ciiCGSWA7SJSU8c", oldPrice: "23.000₫/viên", newPrice: "19.000₫/viên", discount: "-17%" },
                    { name: "Ngói Lợp Đỏ đậm DD09S", driveId: "1vHG-pgeryaSItJoQ5ciiCGSWA7SJSU8c", oldPrice: "23.500₫/viên", newPrice: "19.500₫/viên", discount: "-17%" },
                    { name: "Ngói Lợp Xám tro XT07S", driveId: "1vHG-pgeryaSItJoQ5ciiCGSWA7SJSU8c", oldPrice: "24.000₫/viên", newPrice: "19.800₫/viên", discount: "-18%" },
                    { name: "Ngói Lợp Xanh lá XL02S", driveId: "1vHG-pgeryaSItJoQ5ciiCGSWA7SJSU8c", oldPrice: "24.000₫/viên", newPrice: "19.800₫/viên", discount: "-18%" },
                    { name: "Ngói Lợp Nâu Chocola (socola) NN02S", driveId: "1vHG-pgeryaSItJoQ5ciiCGSWA7SJSU8c", oldPrice: "24.500₫/viên", newPrice: "20.200₫/viên", discount: "-18%" }
                ]
            },
            {
                id: "cat-bon-nuoc",
                title: "BỒN NƯỚC",
                icon: "fa-database",
                subcategories: ["Letton", "Sơn Hà", "Tân Á"],
                products: [
                    { name: "Bồn nước Inox Tân Á TAD2000 (F1340)", driveId: "1X-ECML9CKN4ycBfVFu4pC0wnqzTS12CP", oldPrice: "6.450.000₫", newPrice: "5.290.000₫", discount: "-18%" },
                    { name: "Bồn nhựa đứng Tân Á TA 1000 EX", driveId: "1X-ECML9CKN4ycBfVFu4pC0wnqzTS12CP", oldPrice: "2.450.000₫", newPrice: "1.990.000₫", discount: "-19%" },
                    { name: "Bồn nhựa Tân Á ngang TA 1000 EX", driveId: "1X-ECML9CKN4ycBfVFu4pC0wnqzTS12CP", oldPrice: "2.650.000₫", newPrice: "2.150.000₫", discount: "-19%" },
                    { name: "Bồn nước inox Tân Á 8 đứng 1000 lít TA8D1000 (F940)", driveId: "1X-ECML9CKN4ycBfVFu4pC0wnqzTS12CP", oldPrice: "3.850.000₫", newPrice: "3.150.000₫", discount: "-18%" },
                    { name: "Bồn nhựa Sơn Hà BNMD001000", driveId: "1X-ECML9CKN4ycBfVFu4pC0wnqzTS12CP", oldPrice: "2.550.000₫", newPrice: "2.090.000₫", discount: "-18%" },
                    { name: "Bồn nhựa vân đá đứng Sơn Hà 2000 lít", driveId: "1X-ECML9CKN4ycBfVFu4pC0wnqzTS12CP", oldPrice: "4.950.000₫", newPrice: "4.050.000₫", discount: "-18%" }
                ]
            },
            {
                id: "cat-binh-nong-lanh",
                title: "BÌNH NÓNG LẠNH",
                icon: "fa-temperature-arrow-up",
                subcategories: ["Ariston", "Ferroli"],
                products: [
                    { name: "Máy nước nóng Ariston SB35E-VN 3.5KW", driveId: "1t8U7WQsmDbGWzmSelkxzjVv8M0BvIxAg", oldPrice: "2.650.000₫", newPrice: "2.150.000₫", discount: "-19%" },
                    { name: "Máy nước nóng Ariston Aures SM45PE SBS VN 4.5KW", driveId: "1oah4j6YAPIsJacMYQFJ0JGVemrMwqCgf", oldPrice: "3.450.000₫", newPrice: "2.790.000₫", discount: "-19%" },
                    { name: "Máy nước nóng Ariston AN2 15 R 2.5 FE 15 lít 2.5KW", driveId: "1t8U7WQsmDbGWzmSelkxzjVv8M0BvIxAg", oldPrice: "3.250.000₫", newPrice: "2.650.000₫", discount: "-18%" },
                    { name: "Máy nước nóng Ariston SL2 20 R 2.5FE MT 20 lít 2.5KW", driveId: "1oah4j6YAPIsJacMYQFJ0JGVemrMwqCgf", oldPrice: "3.690.000₫", newPrice: "2.990.000₫", discount: "-19%" },
                    { name: "Máy nước nóng Ferroli QQ Evo 15L ME 15 lít 2.5KW", driveId: "1t8U7WQsmDbGWzmSelkxzjVv8M0BvIxAg", oldPrice: "2.750.000₫", newPrice: "2.250.000₫", discount: "-18%" },
                    { name: "Máy nước nóng Ferroli Divo SSN 4.5S 4.5KW", driveId: "1oah4j6YAPIsJacMYQFJ0JGVemrMwqCgf", oldPrice: "2.550.000₫", newPrice: "2.050.000₫", discount: "-20%" }
                ]
            },
            {
                id: "cat-keo-dan-gach",
                title: "KEO DÁN GẠCH, CHÀ RON",
                icon: "fa-trowel-bricks",
                subcategories: ["Bestmix", "Đồng Tâm", "Keo cá sấu", "Sika"],
                products: [
                    { name: "Vữa rót – Kết nối – Sửa chữa – Hoàn thiện Bestmix", driveId: "15IWAPhzVLsyUO5TDRoWXxvncrHoFcH1_", oldPrice: "340.000₫", newPrice: "275.000₫", discount: "-19%" },
                    { name: "KEO DÁN GẠCH GECKO FLOOR – CHUYÊN LÁT NỀN – BAO 25KG", driveId: "15IWAPhzVLsyUO5TDRoWXxvncrHoFcH1_", oldPrice: "295.000₫", newPrice: "240.000₫", discount: "-19%" },
                    { name: "Sika Tilebond GP – Keo dán gạch đóng bao 25kg", driveId: "17YrxXteZmzhvVRYgfaklNGC2hKjN09N8", oldPrice: "310.000₫", newPrice: "255.000₫", discount: "-18%" },
                    { name: "Keo Chà Ron Crocodile Silver (Keo Cá Sấu Thái Lan)", driveId: "15IWAPhzVLsyUO5TDRoWXxvncrHoFcH1_", oldPrice: "85.000₫", newPrice: "69.000₫", discount: "-19%" }
                ]
            }
        ];

        /* Hàm tạo HTML cho thẻ sản phẩm chuẩn Flatsome (2 cột trên điện thoại, % giảm giá góc trên bên trái, tên không bị tràn hay thiếu chữ) */
        function createFlatsomeProductCard(item) {
            const thumbUrl = `https://drive.google.com/thumbnail?id=${item.driveId || item.id}&sz=w700`;
            const backupUrl = `https://lh3.googleusercontent.com/d/${item.driveId || item.id}=w700`;
            const driveViewUrl = `https://drive.google.com/file/d/${item.driveId || item.id}/view?usp=sharing`;

            return `
                <div class="product-small box" data-drive-url="${driveViewUrl}">
                    <!-- Badge % giảm giá chuẩn Flatsome góc trên bên trái -->
                    <div class="badge-container top left">
                        <div class="onsale-badge">${item.discount}</div>
                    </div>

                    <div>
                        <div class="box-image relative w-full h-36 sm:h-44 bg-slate-100 overflow-hidden border-b border-slate-100">
                            <img src="${thumbUrl}"
                                 onerror="this.onerror=function(){this.src='https://placehold.co/400x400/0f3e68/ffffff?text=MinhHuy.com';};this.src='${backupUrl}';"
                                 alt="${item.name}"
                                 loading="lazy"
                                 class="w-full h-full object-cover">
                        </div>

                        <div class="box-text p-2.5 sm:p-3">
                            <h3 class="product-title-full">${item.name}</h3>
                        </div>
                    </div>

                    <div class="px-2.5 sm:px-3 pb-2.5 sm:pb-3 pt-1 border-t border-slate-100">
                        <div class="price-wrapper flex flex-wrap items-baseline gap-1.5 mb-2">
                            <del class="text-[11px] text-slate-400">${item.oldPrice}</del>
                            <ins class="text-xs sm:text-sm font-extrabold text-[#c81e1e] no-underline">${item.newPrice}</ins>
                        </div>
                        <button type="button" onclick="selectProductForQuote('${item.name.replace(/'/g, "\\'")}')"
                                class="w-full py-1.5 px-2 rounded bg-[#0f3e68] hover:bg-[#1a568e] text-white font-bold text-[11px] sm:text-xs transition text-center">
                            Báo Giá: 0932.555.605
                        </button>
                    </div>
                </div>
            `;
        }

        /* Hiển thị 19 ảnh sản phẩm thực tế từ Google Drive */
        function renderDriveProducts() {
            const grid = document.getElementById("drive-products-grid");
            if (!grid) return;
            grid.innerHTML = driveProductFiles.map(item => createFlatsomeProductCard(item)).join("");
        }

        /* Hiển thị 7 danh mục sản phẩm giống web mẫu noithatngonguyen.com */
        function renderCatalogSections() {
            const container = document.getElementById("catalog-sections-container");
            if (!container) return;

            container.innerHTML = sampleWebsiteCategories.map(section => `
                <section id="${section.id}" class="section-category-block">
                    <div class="flatsome-container">
                        <div class="section-cat-header">
                            <h2 class="section-cat-title">
                                <i class="fa-solid ${section.icon}"></i>${section.title}
                            </h2>
                            <div class="subcat-pills">
                                ${section.subcategories.map(sub => `<a href="#form-bao-gia" class="subcat-pill">${sub}</a>`).join("")}
                                <a href="#form-bao-gia" class="subcat-pill !bg-amber-500 !text-white">Xem thêm &rsaquo;</a>
                            </div>
                        </div>
                        <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-4 gap-3 sm:gap-4">
                            ${section.products.map(prod => createFlatsomeProductCard(prod)).join("")}
                        </div>
                    </div>
                </section>
            `).join("");
        }

        /* Chọn sản phẩm và cuộn xuống Form Báo Giá */
        function selectProductForQuote(productName) {
            const noteInput = document.getElementById("quote-note");
            const formSection = document.getElementById("form-bao-gia");
            if (noteInput) {
                noteInput.value = "Tôi cần tư vấn & nhận báo giá sản phẩm: " + productName;
            }
            if (formSection) {
                formSection.scrollIntoView({ behavior: "smooth" });
            }
        }

        /* Xử lý gửi Form Yêu Cầu Báo Giá */
        function submitQuoteForm(event) {
            event.preventDefault();
            const name = document.getElementById("quote-name").value.trim();
            const phone = document.getElementById("quote-phone").value.trim();
            const category = document.getElementById("quote-category").value;
            const feedback = document.getElementById("quote-feedback");

            if (feedback) {
                feedback.classList.remove("hidden");
                feedback.innerHTML = `Cảm ơn <strong>${name}</strong> (${phone})! Yêu cầu báo giá hạng mục <strong>${category}</strong> đã được ghi nhận tại <strong>minhhuy.com</strong>. Bộ phận kinh doanh Công Ty TNHH Mai Bảo Châu sẽ liên hệ ngay qua SĐT/Zalo <strong>0932.555.605</strong>.`;
            }
        }

        /* Xử lý tìm kiếm sản phẩm */
        function handleProductSearch(event) {
            event.preventDefault();
            const desktopInput = document.getElementById("header-search-input");
            const mobileInput = document.getElementById("mobile-search-input");
            const keyword = ((desktopInput && desktopInput.value) || (mobileInput && mobileInput.value) || "").trim().toLowerCase();

            if (!keyword) return;

            const allCards = document.querySelectorAll(".product-small.box");
            let firstMatch = null;
            allCards.forEach(card => {
                const text = card.innerText.toLowerCase();
                if (text.includes(keyword)) {
                    card.style.outline = "2px solid #d97706";
                    if (!firstMatch) firstMatch = card;
                } else {
                    card.style.outline = "none";
                }
            });

            if (firstMatch) {
                firstMatch.scrollIntoView({ behavior: "smooth", block: "center" });
            }
        }

        /* Điều khiển 2 Banner tự trượt chuyên nghiệp */
        let currentSlideIndex = 0;
        let bannerInterval = null;

        function showBannerSlide(index) {
            const slides = document.querySelectorAll(".banner-slide");
            const dots = document.querySelectorAll(".banner-dot");
            if (!slides.length) return;

            currentSlideIndex = (index + slides.length) % slides.length;
            slides.forEach((slide, i) => {
                slide.classList.toggle("active", i === currentSlideIndex);
            });
            dots.forEach((dot, i) => {
                dot.className = i === currentSlideIndex
                    ? "banner-dot w-2.5 h-2.5 rounded-full bg-amber-400 transition"
                    : "banner-dot w-2.5 h-2.5 rounded-full bg-white/50 transition";
            });
        }

        function changeBannerSlide(step) {
            showBannerSlide(currentSlideIndex + step);
            restartBannerAutoSlide();
        }

        function goToBannerSlide(index) {
            showBannerSlide(index);
            restartBannerAutoSlide();
        }

        function restartBannerAutoSlide() {
            if (bannerInterval) clearInterval(bannerInterval);
            bannerInterval = setInterval(() => {
                showBannerSlide(currentSlideIndex + 1);
            }, 5000);
        }

        /* Đóng/Mở Menu trên điện thoại */
        function closeMobileMenu() {
            const drawer = document.getElementById("mobile-drawer");
            if (drawer) drawer.classList.add("hidden");
        }

        window.onload = function () {
            renderDriveProducts();
            renderCatalogSections();
            restartBannerAutoSlide();

            const openBtn = document.getElementById("mobile-menu-btn");
            const closeBtn = document.getElementById("close-mobile-menu");
            const drawer = document.getElementById("mobile-drawer");

            if (openBtn && drawer) {
                openBtn.addEventListener("click", () => drawer.classList.remove("hidden"));
            }
            if (closeBtn) {
                closeBtn.addEventListener("click", closeMobileMenu);
            }
            if (drawer) {
                drawer.addEventListener("click", (e) => {
                    if (e.target === drawer) closeMobileMenu();
                });
            }
        };
    </script>
</body>
</html>
