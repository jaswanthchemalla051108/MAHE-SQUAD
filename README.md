<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>MAHE Bengaluru | Batch 2026 - 2030 Vault</title>
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- Lucide Icons -->
  <script src="https://unpkg.com/lucide@latest"></script>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap');
    body {
      font-family: 'Plus Jakarta Sans', sans-serif;
    }
    .custom-scrollbar::-webkit-scrollbar {
      width: 6px;
    }
    .custom-scrollbar::-webkit-scrollbar-track {
      background: rgba(255, 255, 255, 0.05);
    }
    .custom-scrollbar::-webkit-scrollbar-thumb {
      background: rgba(255, 255, 255, 0.2);
      border-radius: 9999px;
    }
  </style>
</head>
<body class="bg-slate-950 text-slate-100 min-h-screen flex flex-col selection:bg-amber-500 selection:text-slate-950">

  <!-- Top Announcement / Batch Badge -->
  <div class="bg-gradient-to-r from-amber-600 via-rose-600 to-indigo-600 text-white text-xs font-semibold py-1.5 px-4 text-center tracking-wider uppercase flex items-center justify-center gap-2 shadow-inner">
    <span class="inline-block w-2 h-2 rounded-full bg-emerald-300 animate-pulse"></span>
    MAHE Bengaluru • CSE Official Memory Vault • Batch 2026 – 2030
  </div>

  <!-- Navbar -->
  <header class="sticky top-0 z-40 bg-slate-900/80 backdrop-blur-md border-b border-slate-800">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 py-3.5 flex flex-wrap items-center justify-between gap-4">
      
      <!-- Brand & Squad Details -->
      <div class="flex items-center gap-3">
        <div class="w-10 h-10 rounded-xl bg-gradient-to-br from-amber-500 to-rose-600 flex items-center justify-center shadow-lg shadow-rose-900/30 ring-2 ring-white/10">
          <i data-lucide="sparkles" class="w-5 h-5 text-white"></i>
        </div>
        <div>
          <div class="flex items-center gap-2">
            <h1 class="text-base sm:text-lg font-bold tracking-tight text-white">The Quad Vault</h1>
            <span class="text-[10px] uppercase font-extrabold px-2 py-0.5 rounded-full bg-amber-500/20 text-amber-400 border border-amber-500/30">
              '26–'30
            </span>
          </div>
          <p class="text-xs text-slate-400">Jaswanth • Sampreeth • Akhila • Sahithi</p>
        </div>
      </div>

      <!-- Quick Actions -->
      <div class="flex items-center gap-2.5 sm:gap-3">
        <!-- Identity Selector -->
        <div class="flex items-center gap-1.5 bg-slate-800/80 border border-slate-700/60 rounded-xl px-2.5 py-1.5 text-xs text-slate-300">
          <span class="text-slate-400 hidden sm:inline">Active:</span>
          <select id="activeUserSelect" class="bg-transparent text-amber-400 font-semibold focus:outline-none cursor-pointer">
            <option value="Jaswanth" class="bg-slate-900 text-slate-100">Jaswanth</option>
            <option value="Sampreeth" class="bg-slate-900 text-slate-100">Sampreeth</option>
            <option value="Akhila" class="bg-slate-900 text-slate-100">Akhila</option>
            <option value="Sahithi" class="bg-slate-900 text-slate-100">Sahithi</option>
          </select>
        </div>

        <!-- Add Photo Button -->
        <button onclick="openUploadModal()" class="flex items-center gap-1.5 bg-gradient-to-r from-amber-500 to-amber-600 hover:from-amber-400 hover:to-amber-500 text-slate-950 font-bold text-xs sm:text-sm px-3.5 py-2 rounded-xl shadow-lg shadow-amber-500/20 transition active:scale-95">
          <i data-lucide="plus-circle" class="w-4 h-4"></i>
          <span>Upload</span>
        </button>

        <!-- Deploy Info Button -->
        <button onclick="openDeployModal()" class="flex items-center gap-1.5 bg-slate-800 hover:bg-slate-700 text-slate-200 text-xs sm:text-sm font-medium px-3 py-2 rounded-xl border border-slate-700 transition">
          <i data-lucide="globe" class="w-4 h-4 text-emerald-400"></i>
          <span class="hidden sm:inline">Launch</span> .fun
        </button>
      </div>
    </div>
  </header>

  <!-- Main Container -->
  <main class="max-w-6xl mx-auto px-4 sm:px-6 py-6 flex-1 w-full space-y-6">

    <!-- Squad Profile Cards -->
    <section class="grid grid-cols-2 md:grid-cols-4 gap-3 sm:gap-4">
      <!-- Member 1: Jaswanth -->
      <div class="bg-slate-900/60 border border-slate-800 rounded-2xl p-3.5 flex items-center gap-3 hover:border-slate-700 transition">
        <div class="w-11 h-11 rounded-full bg-gradient-to-tr from-cyan-500 to-blue-600 flex items-center justify-center font-bold text-sm text-white shadow-md">
          JA
        </div>
        <div class="min-w-0">
          <h3 class="text-sm font-bold text-slate-100 truncate">Jaswanth</h3>
          <p class="text-[11px] text-slate-400 truncate">Tech & Lens</p>
        </div>
      </div>

      <!-- Member 2: Sampreeth -->
      <div class="bg-slate-900/60 border border-slate-800 rounded-2xl p-3.5 flex items-center gap-3 hover:border-slate-700 transition">
        <div class="w-11 h-11 rounded-full bg-gradient-to-tr from-amber-500 to-orange-600 flex items-center justify-center font-bold text-sm text-white shadow-md">
          SA
        </div>
        <div class="min-w-0">
          <h3 class="text-sm font-bold text-slate-100 truncate">Sampreeth</h3>
          <p class="text-[11px] text-slate-400 truncate">Campus Vibes & Food</p>
        </div>
      </div>

      <!-- Member 3: Akhila -->
      <div class="bg-slate-900/60 border border-slate-800 rounded-2xl p-3.5 flex items-center gap-3 hover:border-slate-700 transition">
        <div class="w-11 h-11 rounded-full bg-gradient-to-tr from-rose-500 to-pink-600 flex items-center justify-center font-bold text-sm text-white shadow-md">
          AK
        </div>
        <div class="min-w-0">
          <h3 class="text-sm font-bold text-slate-100 truncate">Akhila</h3>
          <p class="text-[11px] text-slate-400 truncate">Creative & Photos</p>
        </div>
      </div>

      <!-- Member 4: Sahithi -->
      <div class="bg-slate-900/60 border border-slate-800 rounded-2xl p-3.5 flex items-center gap-3 hover:border-slate-700 transition">
        <div class="w-11 h-11 rounded-full bg-gradient-to-tr from-emerald-500 to-teal-600 flex items-center justify-center font-bold text-sm text-white shadow-md">
          SH
        </div>
        <div class="min-w-0">
          <h3 class="text-sm font-bold text-slate-100 truncate">Sahithi</h3>
          <p class="text-[11px] text-slate-400 truncate">Navigator & Events</p>
        </div>
      </div>
    </section>

    <!-- Filter & Search Bar -->
    <section class="bg-slate-900/50 border border-slate-800/80 rounded-2xl p-4 flex flex-wrap items-center justify-between gap-3">
      <div class="flex flex-wrap items-center gap-2">
        <button onclick="filterPhotos('all')" class="filter-btn px-3 py-1.5 rounded-lg text-xs font-semibold bg-amber-500 text-slate-950 transition active:scale-95" data-filter="all">
          All Memories
        </button>
        <button onclick="filterPhotos('Central Lawn')" class="filter-btn px-3 py-1.5 rounded-lg text-xs font-semibold bg-slate-800 hover:bg-slate-700 text-slate-300 transition" data-filter="Central Lawn">
          Central Lawn
        </button>
        <button onclick="filterPhotos('Food Court')" class="filter-btn px-3 py-1.5 rounded-lg text-xs font-semibold bg-slate-800 hover:bg-slate-700 text-slate-300 transition" data-filter="Food Court">
          Food Court
        </button>
        <button onclick="filterPhotos('Academic Block')" class="filter-btn px-3 py-1.5 rounded-lg text-xs font-semibold bg-slate-800 hover:bg-slate-700 text-slate-300 transition" data-filter="Academic Block">
          Academic Block
        </button>
        <button onclick="filterPhotos('Hostel Courtyard')" class="filter-btn px-3 py-1.5 rounded-lg text-xs font-semibold bg-slate-800 hover:bg-slate-700 text-slate-300 transition" data-filter="Hostel Courtyard">
          Hostel Courtyard
        </button>
      </div>

      <div class="text-xs text-slate-400 font-medium flex items-center gap-1.5">
        <i data-lucide="camera" class="w-3.5 h-3.5 text-amber-400"></i>
        <span id="photoCount">0 Photos Logged</span>
      </div>
    </section>

    <!-- Photo Feed Gallery -->
    <section id="galleryGrid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-5">
      <!-- Injected via JavaScript -->
    </section>

    <!-- Empty State (if needed) -->
    <div id="emptyState" class="hidden text-center py-16">
      <i data-lucide="image" class="w-12 h-12 mx-auto text-slate-600 mb-3"></i>
      <p class="text-base text-slate-300 font-medium">No photos found for this spot yet.</p>
      <p class="text-xs text-slate-500 mt-1">Click the Upload button above to add your first memory!</p>
    </div>
  </main>

  <!-- Upload Modal -->
  <div id="uploadModal" class="fixed inset-0 bg-black/80 backdrop-blur-sm z-50 hidden flex items-center justify-center p-4">
    <div class="bg-slate-900 border border-slate-800 rounded-3xl w-full max-w-md p-6 relative shadow-2xl">
      <button onclick="closeUploadModal()" class="absolute top-4 right-4 text-slate-400 hover:text-white p-1">
        <i data-lucide="x" class="w-5 h-5"></i>
      </button>

      <div class="flex items-center gap-2 mb-4">
        <div class="w-8 h-8 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center">
          <i data-lucide="upload" class="w-4 h-4"></i>
        </div>
        <h3 class="text-lg font-bold text-white">Add Campus Memory</h3>
      </div>

      <form id="memoryForm" onsubmit="handleMemorySubmit(event)" class="space-y-4">
        <!-- Image Upload / Drag Drop -->
        <div>
          <label class="block text-xs font-semibold text-slate-300 mb-1">Upload Photo</label>
          <div class="border-2 border-dashed border-slate-700 hover:border-amber-500 rounded-2xl p-4 text-center cursor-pointer transition relative bg-slate-950/40">
            <input type="file" id="photoInput" accept="image/*" required class="absolute inset-0 opacity-0 cursor-pointer" onchange="previewImage(event)" />
            <div id="uploadPlaceholder" class="flex flex-col items-center">
              <i data-lucide="image-plus" class="w-8 h-8 text-slate-400 mb-2"></i>
              <span class="text-xs text-slate-300 font-medium">Click or drag photo here</span>
              <span class="text-[10px] text-slate-500 mt-0.5">JPG, PNG, WebP supported</span>
            </div>
            <img id="imagePreview" class="hidden rounded-xl max-h-44 mx-auto object-cover" />
          </div>
        </div>

        <!-- Campus Spot Selection -->
        <div>
          <label class="block text-xs font-semibold text-slate-300 mb-1">Campus Spot</label>
          <select id="spotInput" class="w-full bg-slate-800 border border-slate-700 text-slate-200 text-xs rounded-xl p-2.5 focus:outline-none focus:border-amber-500">
            <option value="Central Lawn">Central Lawn</option>
            <option value="Food Court">Food Court / Canteen</option>
            <option value="Academic Block">Academic Block & Labs</option>
            <option value="Hostel Courtyard">Hostel Courtyard</option>
            <option value="Sports Arena">Sports Arena</option>
            <option value="Off-Campus Hangout">Off-Campus Hangout</option>
          </select>
        </div>

        <!-- Caption -->
        <div>
          <label class="block text-xs font-semibold text-slate-300 mb-1">Caption / Story</label>
          <textarea id="captionInput" rows="2" required placeholder="What was happening here?" class="w-full bg-slate-800 border border-slate-700 text-slate-200 text-xs rounded-xl p-2.5 focus:outline-none focus:border-amber-500 placeholder-slate-500"></textarea>
        </div>

        <!-- Submit Button -->
        <button type="submit" class="w-full py-2.5 bg-gradient-to-r from-amber-500 to-amber-600 hover:from-amber-400 hover:to-amber-500 text-slate-950 font-bold text-sm rounded-xl shadow-lg transition active:scale-95">
          Save to 2026–2030 Vault
        </button>
      </form>
    </div>
  </div>

  <!-- Deploy Guide Modal (.FUN & GitHub Education) -->
  <div id="deployModal" class="fixed inset-0 bg-black/80 backdrop-blur-sm z-50 hidden flex items-center justify-center p-4">
    <div class="bg-slate-900 border border-slate-800 rounded-3xl w-full max-w-lg p-6 relative shadow-2xl max-h-[90vh] overflow-y-auto custom-scrollbar">
      <button onclick="closeDeployModal()" class="absolute top-4 right-4 text-slate-400 hover:text-white p-1">
        <i data-lucide="x" class="w-5 h-5"></i>
      </button>

      <div class="flex items-center gap-2.5 mb-4">
        <div class="w-9 h-9 rounded-xl bg-emerald-500/20 text-emerald-400 flex items-center justify-center">
          <i data-lucide="rocket" class="w-5 h-5"></i>
        </div>
        <div>
          <h3 class="text-base font-bold text-white">Deploying on your .FUN Domain</h3>
          <p class="text-xs text-slate-400">Zero cost with GitHub Student Developer Pack</p>
        </div>
      </div>

      <div class="space-y-4 text-xs text-slate-300 leading-relaxed">
        <div class="bg-slate-800/60 p-3.5 rounded-2xl border border-slate-700/60 space-y-1">
          <span class="font-bold text-amber-400 block">Step 1: Put Code on GitHub</span>
          <p class="text-slate-400">Create a new repository called <code class="text-white bg-slate-900 px-1 py-0.5 rounded">campus-vault</code> and upload this <code class="text-white bg-slate-900 px-1 py-0.5 rounded">index.html</code> file.</p>
        </div>

        <div class="bg-slate-800/60 p-3.5 rounded-2xl border border-slate-700/60 space-y-1">
          <span class="font-bold text-amber-400 block">Step 2: Claim your Domain</span>
          <p class="text-slate-400">Open your <strong>GitHub Student Developer Pack</strong> dashboard. Claim your free domain voucher on Namecheap (free .me) or Name.com (free 1-year registration). If you want <strong>.fun</strong>, you can pick it up via Name.com offer or grab it on Namecheap for under ₹100.</p>
        </div>

        <div class="bg-slate-800/60 p-3.5 rounded-2xl border border-slate-700/60 space-y-1">
          <span class="font-bold text-amber-400 block">Step 3: Connect to Vercel (Recommended)</span>
          <p class="text-slate-400">Log into <strong>vercel.com</strong> with GitHub &rarr; Import your <code class="text-white bg-slate-900 px-1 py-0.5 rounded">campus-vault</code> repository &rarr; Click Deploy. Under <em>Project Settings &gt; Domains</em>, type your <code class="text-amber-400">.fun</code> domain and copy the DNS records to your registrar.</p>
        </div>

        <div class="bg-slate-800/60 p-3.5 rounded-2xl border border-slate-700/60 space-y-1">
          <span class="font-bold text-amber-400 block">Step 4: Grant Access to All 4</span>
          <p class="text-slate-400">Add <strong>Sampreeth</strong>, <strong>Akhila</strong>, and <strong>Sahithi</strong> as Collaborators in your GitHub repository so all 4 of you have full push access.</p>
        </div>
      </div>
    </div>
  </div>

  <!-- Footer -->
  <footer class="mt-auto border-t border-slate-800/80 py-5 text-center text-xs text-slate-500">
    MAHE Bengaluru • CSE Batch 2026 – 2030 Memory Vault • Built for the 4
  </footer>

  <!-- Application Logic -->
  <script>
    // Initial sample dataset for the 4 friends
    const defaultMemories = [
      {
        id: 1,
        author: "Jaswanth",
        spot: "Academic Block",
        caption: "First day setting up VS Code in the lab. Batch 2026-2030 officially kickstarted!",
        date: "Sep 2026",
        likes: 3,
        liked: false,
        img: "https://images.unsplash.com/photo-1523240795612-9a054b0db644?auto=format&fit=crop&w=800&q=80"
      },
      {
        id: 2,
        author: "Sampreeth",
        spot: "Food Court",
        caption: "Post-lecture mess break. The samosas and chai hit different today.",
        date: "Sep 2026",
        likes: 3,
        liked: false,
        img: "https://images.unsplash.com/photo-1517248135467-4c7edcad34c4?auto=format&fit=crop&w=800&q=80"
      },
      {
        id: 3,
        author: "Akhila",
        spot: "Central Lawn",
        caption: "Golden hour after classes. Getting our group photos sorted for the year.",
        date: "Sep 2026",
        likes: 4,
        liked: false,
        img: "https://images.unsplash.com/photo-1541339907198-e08756dedf3f?auto=format&fit=crop&w=800&q=80"
      },
      {
        id: 4,
        author: "Sahithi",
        spot: "Hostel Courtyard",
        caption: "Hostel hangout planning the upcoming weekend. 4 more years of this!",
        date: "Sep 2026",
        likes: 3,
        liked: false,
        img: "https://images.unsplash.com/photo-1529156069898-49953e39b3ac?auto=format&fit=crop&w=800&q=80"
      }
    ];

    let memories = JSON.parse(localStorage.getItem('mahe_squad_memories')) || defaultMemories;
    let currentFilter = 'all';

    function saveMemories() {
      localStorage.setItem('mahe_squad_memories', JSON.stringify(memories));
    }

    function renderGallery() {
      const gallery = document.getElementById('galleryGrid');
      const emptyState = document.getElementById('emptyState');
      const photoCount = document.getElementById('photoCount');
      
      const filtered = currentFilter === 'all' 
        ? memories 
        : memories.filter(m => m.spot.toLowerCase().includes(currentFilter.toLowerCase()));

      photoCount.innerText = `${filtered.length} Photo${filtered.length === 1 ? '' : 's'} Logged`;

      if (filtered.length === 0) {
        gallery.innerHTML = '';
        emptyState.classList.remove('hidden');
        return;
      }

      emptyState.classList.add('hidden');
      gallery.innerHTML = filtered.map(item => `
        <article class="bg-slate-900/70 border border-slate-800/80 rounded-3xl overflow-hidden hover:border-slate-700 transition flex flex-col group shadow-lg">
          <div class="relative aspect-video overflow-hidden bg-slate-950">
            <img src="${item.img}" alt="${item.caption}" class="w-full h-full object-cover group-hover:scale-105 transition duration-500" />
            <span class="absolute top-3 left-3 px-2.5 py-1 rounded-full text-[10px] font-bold uppercase tracking-wider bg-black/60 backdrop-blur-md text-amber-400 border border-white/10">
              ${item.spot}
            </span>
          </div>
          <div class="p-4 flex-1 flex flex-col justify-between space-y-3">
            <div>
              <div class="flex items-center justify-between text-xs text-slate-400 mb-1.5">
                <span class="font-bold text-slate-200">${item.author}</span>
                <span class="text-[11px] text-slate-500">${item.date}</span>
              </div>
              <p class="text-xs text-slate-300 leading-relaxed">${item.caption}</p>
            </div>

            <div class="pt-2 border-t border-slate-800/70 flex items-center justify-between">
              <button onclick="toggleLike(${item.id})" class="flex items-center gap-1.5 text-xs font-semibold ${item.liked ? 'text-rose-500' : 'text-slate-400 hover:text-rose-400'} transition">
                <i data-lucide="heart" class="w-4 h-4 ${item.liked ? 'fill-rose-500' : ''}"></i>
                <span>${item.likes}</span>
              </button>
              <span class="text-[10px] uppercase font-bold text-slate-500 tracking-wider">MAHE '26–'30</span>
            </div>
          </div>
        </article>
      `).join('');

      lucide.createIcons();
    }

    function toggleLike(id) {
      memories = memories.map(m => {
        if (m.id === id) {
          return {
            ...m,
            liked: !m.liked,
            likes: m.liked ? m.likes - 1 : m.likes + 1
          };
        }
        return m;
      });
      saveMemories();
      renderGallery();
    }

    function filterPhotos(spot) {
      currentFilter = spot;
      document.querySelectorAll('.filter-btn').forEach(btn => {
        if (btn.getAttribute('data-filter') === spot) {
          btn.className = 'filter-btn px-3 py-1.5 rounded-lg text-xs font-semibold bg-amber-500 text-slate-950 transition active:scale-95';
        } else {
          btn.className = 'filter-btn px-3 py-1.5 rounded-lg text-xs font-semibold bg-slate-800 hover:bg-slate-700 text-slate-300 transition';
        }
      });
      renderGallery();
    }

    let uploadedBase64 = null;

    function previewImage(event) {
      const file = event.target.files[0];
      if (file) {
        const reader = new FileReader();
        reader.onload = function(e) {
          uploadedBase64 = e.target.result;
          document.getElementById('uploadPlaceholder').classList.add('hidden');
          const preview = document.getElementById('imagePreview');
          preview.src = uploadedBase64;
          preview.classList.remove('hidden');
        };
        reader.readAsDataURL(file);
      }
    }

    function handleMemorySubmit(e) {
      e.preventDefault();
      if (!uploadedBase64) return;

      const activeUser = document.getElementById('activeUserSelect').value;
      const spot = document.getElementById('spotInput').value;
      const caption = document.getElementById('captionInput').value;

      const newMemory = {
        id: Date.now(),
        author: activeUser,
        spot: spot,
        caption: caption,
        date: "Batch 2026-30",
        likes: 1,
        liked: true,
        img: uploadedBase64
      };

      memories.unshift(newMemory);
      saveMemories();
      renderGallery();
      closeUploadModal();
      document.getElementById('memoryForm').reset();
      document.getElementById('uploadPlaceholder').classList.remove('hidden');
      document.getElementById('imagePreview').classList.add('hidden');
      uploadedBase64 = null;
    }

    function openUploadModal() {
      document.getElementById('uploadModal').classList.remove('hidden');
    }
    function closeUploadModal() {
      document.getElementById('uploadModal').classList.add('hidden');
    }
    function openDeployModal() {
      document.getElementById('deployModal').classList.remove('hidden');
    }
    function closeDeployModal() {
      document.getElementById('deployModal').classList.add('hidden');
    }

    // Initialize
    renderGallery();
    lucide.createIcons();
  </script>
</body>
</html>
