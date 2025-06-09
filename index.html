import React, { useState, useEffect, useCallback, useReducer, useMemo } from 'react';
import { Home, Briefcase, BookOpen, Handshake, User, Search, CheckCircle, Lightbulb, MapPin, DollarSign, Heart, X, Info, TrendingUp, Star, Zap, ChevronLeft, ChevronRight, Sparkles, Key, Mail, LogOut, Award, ShieldCheck, Wallet, SlidersHorizontal, BarChart2, FileText, Send, Eye, Clock, MessageSquare, CalendarPlus, Settings, Building, FileBadge2, Bell, Moon, Sun } from 'lucide-react';

// ===================================================================================
// 1. MOCK DATA & UTILITIES
// ===================================================================================

const mockJobs = [
    { id: 'j1', title: 'Spesialis Pemasaran Digital', company: 'Inovasi Digital Nusantara', location: 'Jakarta', salary: 'Rp 7jt - 10jt', jobType: 'Full-time', benefits: ['Jaminan Kesehatan', 'Dana Pensiun', 'Cuti Tahunan', 'Pengembangan Karir'], decentWorkCriteria: { salary: 5, benefits: 5, transparency: 4, development: 4 }, isDecentWork: true, description: 'Mencari spesialis pemasaran digital yang kreatif dan berbasis data untuk mengelola semua kampanye digital kami.', requirements: ['S1 Pemasaran/Komunikasi', '2+ tahun pengalaman di SEO/SEM', 'Mahir Google Analytics'], image: 'https://placehold.co/400x200/a8dadc/1d3557?text=Marketing', companyLogo: 'https://placehold.co/100x100/1d3557/ffffff?text=IDN', category: 'Pemasaran' },
    { id: 'j2', title: 'Pengembang Perangkat Lunak', company: 'Teknologi Maju Bersama', location: 'Bandung', salary: 'Rp 9jt - 15jt', jobType: 'Full-time', benefits: ['Jaminan Kesehatan', 'Dana Pensiun', 'Makan Siang Gratis', 'Jam Kerja Fleksibel'], decentWorkCriteria: { salary: 5, benefits: 5, transparency: 5, development: 5 }, isDecentWork: true, description: 'Kami mencari pengembang fullstack yang berbakat untuk membangun fitur-fitur inovatif pada platform kami.', requirements: ['S1 Ilmu Komputer', '3+ tahun pengalaman dengan React & Node.js', 'Menguasai database SQL/NoSQL'], image: 'https://placehold.co/400x200/f4a261/2a9d8f?text=Software+Dev', companyLogo: 'https://placehold.co/100x100/2a9d8f/ffffff?text=TMB', category: 'Teknologi' },
    { id: 'j3', title: 'Asisten Administrasi', company: 'Solusi Kantor Cepat', location: 'Surabaya', salary: 'Rp 4jt - 6jt', jobType: 'Full-time', benefits: ['Jaminan Kesehatan'], decentWorkCriteria: { salary: 4, benefits: 2, transparency: 3, development: 2 }, isDecentWork: false, description: 'Membutuhkan asisten administrasi yang teliti dan terorganisir untuk mendukung operasional harian.', requirements: ['SMA/SMK', 'Minimal 1 tahun pengalaman administrasi', 'Mahir menggunakan MS Office'], image: 'https://placehold.co/400x200/e9c46a/264653?text=Admin', companyLogo: 'https://placehold.co/100x100/264653/ffffff?text=SKC', category: 'Administrasi' },
    { id: 'j7', title: 'Product Manager', company: 'Startup Cepat Naik', location: 'Jakarta', salary: 'Rp 12jt - 18jt', jobType: 'Full-time', benefits: ['Jaminan Kesehatan', 'Dana Pensiun', 'Opsi Saham', 'Anggaran Belajar'], decentWorkCriteria: { salary: 5, benefits: 4, transparency: 5, development: 5 }, isDecentWork: true, description: 'Memimpin siklus hidup produk dari ide hingga peluncuran, bekerja sama dengan tim teknik, desain, dan pemasaran.', requirements: ['S1 Bisnis/Teknik', '3+ tahun pengalaman sebagai Product Manager', 'Berpengalaman dengan Agile/Scrum'], image: 'https://placehold.co/400x200/457b9d/e0fbfc?text=Product+Manager', companyLogo: 'https://placehold.co/100x100/457b9d/ffffff?text=SCN', category: 'Produk' },
    { id: 'j8', title: 'UI/UX Designer', company: 'Desain Interaktif', location: 'Yogyakarta', salary: 'Rp 8jt - 12jt', jobType: 'Full-time', benefits: ['Jaminan Kesehatan', 'Alat Kerja Terbaru', 'Suasana Kerja Santai'], decentWorkCriteria: { salary: 5, benefits: 4, transparency: 4, development: 4 }, isDecentWork: true, description: 'Menciptakan pengalaman pengguna yang intuitif dan menarik secara visual untuk produk digital kami.', requirements: ['Memiliki portofolio yang kuat', '2+ tahun pengalaman desain produk', 'Mahir Figma/Sketch'], image: 'https://placehold.co/400x200/e07a5f/f4f1de?text=UI/UX+Design', companyLogo: 'https://placehold.co/100x100/e07a5f/ffffff?text=DI', category: 'Desain' },
];
const mockCourses = [
    { id: 'c1', title: 'Dasar-Dasar Pemasaran Digital', provider: 'Akademi Digital', level: 'Pemula', price: 'Gratis', isPaid: false, description: 'Pelajari strategi inti pemasaran digital dari SEO, SEM, hingga media sosial untuk memulai karir Anda.', link: '#', image: 'https://placehold.co/400x200/8ecae6/023047?text=Learn+Digital', category: 'Pemasaran', schedule: {day: 'Senin', time: '09:00 WIB'} },
    { id: 'c2', title: 'Pengembangan Web dengan React.js', provider: 'CoderHub', level: 'Menengah', price: 'Rp 1.500.000', isPaid: true, description: 'Kursus mendalam tentang membangun aplikasi web interaktif dan modern menggunakan React.js dan ekosistemnya.', link: '#', image: 'https://placehold.co/400x200/219ebc/023047?text=React+Mastery', category: 'Teknologi', schedule: {day: 'Selasa', time: '13:00 WIB'} },
    { id: 'c3', title: 'Manajemen Produk untuk Pemula', provider: 'Pusat Inovasi', level: 'Pemula', price: 'Gratis', isPaid: false, description: 'Panduan praktis untuk menjadi manajer produk yang sukses, dari riset pasar hingga peluncuran produk.', link: '#', image: 'https://placehold.co/400x200/fb8500/023047?text=Product+101', category: 'Produk', schedule: {day: 'Rabu', time: '10:00 WIB'} },
    { id: 'c4', title: 'Masterclass Desain UI/UX', provider: 'Desain Hebat', level: 'Menengah', price: 'Rp 2.000.000', isPaid: true, description: 'Tingkatkan skill desain Anda ke level selanjutnya dengan studi kasus nyata dan proyek langsung.', link: '#', image: 'https://placehold.co/400x200/ffb703/023047?text=UX+Mastery', category: 'Desain', schedule: {day: 'Kamis', time: '14:00 WIB'} },
];
const mockUmkm = [
    { id: 'u1', name: 'Kopi Nusantara', category: 'Kuliner', location: 'Jakarta', description: 'Kedai kopi lokal yang berkomitmen menggunakan biji kopi dari petani lokal dan mempraktikkan upah layak.', isSustainable: true, image: 'https://placehold.co/400x200/0077b6/ffffff?text=Local+Coffee', rating: 4.8, reviews: 124 },
    { id: 'u2', name: 'Batik Tradisi', category: 'Fashion & Kerajinan', location: 'Yogyakarta', description: 'Produsen batik tulis tangan yang memberdayakan pengrajin lokal dan menggunakan pewarna alami.', isSustainable: true, image: 'https://placehold.co/400x200/00b4d8/ffffff?text=Handmade+Batik', rating: 4.9, reviews: 89 },
    { id: 'u3', name: 'Bengkel Sehat', category: 'Otomotif', location: 'Surabaya', description: 'Bengkel mobil dengan teknisi bersertifikat dan harga transparan untuk semua layanan.', isSustainable: false, image: 'https://placehold.co/400x200/90e0ef/0077b6?text=Auto+Service', rating: 4.5, reviews: 210 },
];
const userProfile = {
    name: "Rina S.",
    email: "rina.s@email.com",
    avatar: "https://i.pravatar.cc/150?u=a042581f4e29026704d",
    interests: ["Teknologi", "Desain"],
    savedJobIds: ['j2', 'j8', 'j7'],
    savedCourseIds: ['c2'],
    workHistory: [
        { company: "Tech Solutions Inc.", position: "Junior Web Developer", period: "2022 - 2024", rating: 4.5, comment: "Rina adalah anggota tim yang proaktif dan cepat belajar. Kontribusinya pada proyek utama kami sangat signifikan." },
        { company: "Creative Agency", position: "UI/UX Intern", period: "2021", rating: 5, comment: "Menunjukkan bakat desain yang luar biasa dan kemampuan kolaborasi yang sangat baik." }
    ]
};

const FontImports = () => ( <><link rel="preconnect" href="https://fonts.googleapis.com" /><link rel="preconnect" href="https://fonts.gstatic.com" crossOrigin="true" /><link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Poppins:wght@600;700;800&display=swap" rel="stylesheet" /></> );
const calculateDecentWorkScore = (c) => c ? Math.round(((c.salary||0)+(c.benefits||0)+(c.transparency||0)+(c.development||0))/2)/2 : 0;
const StarRating = ({ score, size = 16, className = '' }) => { const s = [...Array(5)].map((_, i) => i < score ? (i < Math.floor(score) ? 'full' : 'half') : 'empty'); return <div className={`flex items-center text-amber-400 ${className}`}>{s.map((type, i) => <Star key={i} size={size} fill={type !== 'empty' ? 'currentColor' : 'none'} className={type === 'empty' ? 'text-gray-300' : ''} style={type === 'half' ? {clipPath: 'polygon(0 0, 50% 0, 50% 100%, 0 100%)'} : {}}/>)}</div>; };
const Toast = ({ message, show, type }) => !show ? null : <div className={`fixed bottom-20 md:bottom-5 left-1/2 -translate-x-1/2 z-50 px-4 py-2 rounded-lg shadow-lg animate-fade-in-out ${type === 'success' ? 'bg-emerald-600' : type === 'error' ? 'bg-red-600' : 'bg-slate-800'} text-white`}>{message}</div>;
function useToast() { const [t, setT] = useState({ message: '', show: false, type: 'info' }); const showT = useCallback((m,t='info',d=3000)=>{setT({message:m,show:true,type:t});setTimeout(()=>setT(p=>({...p,show:false})),d)},[]); return [t, showT]; }
const callGeminiAPI = async (prompt, apiKey) => { try { const r = await fetch(`https://generativelanguage.googleapis.com/v1beta/models/gemini-1.5-flash:generateContent?key=${apiKey}`,{method:'POST',headers:{'Content-Type':'application/json'},body:JSON.stringify({contents:[{role:"user",parts:[{text:prompt}]}]})}); if(!r.ok) throw new Error(r.status); const j = await r.json(); return j.candidates?.[0]?.content?.parts?.[0]?.text||"AI tidak memberi respons.";} catch(e){console.error(e);return "Gagal menghubungi AI."}};
const generateICSFile = (event) => { const formatDate = (date) => date.toISOString().replace(/[-:]/g, '').split('.')[0] + 'Z'; const icsContent = ['BEGIN:VCALENDAR', 'VERSION:2.0', 'PRODID:-//KerjaKita//App//EN', 'BEGIN:VEVENT', `UID:${new Date().getTime()}@kerjakita.com`, `DTSTAMP:${formatDate(new Date())}`, `DTSTART:${formatDate(event.startTime)}`, `DTEND:${formatDate(event.endTime)}`, `SUMMARY:${event.title}`, `DESCRIPTION:${event.description}`, `LOCATION:${event.location}`, 'END:VEVENT', 'END:VCALENDAR'].join('\n'); return `data:text/calendar;charset=utf8,${encodeURIComponent(icsContent)}`; };

// ===================================================================================
// 4. CORE PAGES & COMPONENTS
// ===================================================================================

const initialFilterState = { searchTerm: '', sortBy: 'relevance', jobTypeFilter: '', showDecentWorkOnly: false, courseLevelFilter: '', coursePriceFilter: '', courseCategoryFilter: '', umkmSustainableOnly: false };
function filterReducer(state, action) { if (action.type === 'SET_FILTER') return { ...state, [action.payload.key]: action.payload.value }; if (action.type === 'RESET_FILTERS') return initialFilterState; return state; }

const ApplicationStatus = { DILAMAR: 'Dilamar', DITINJAU: 'Ditinjau', WAWANCARA: 'Wawancara', DITERIMA: 'Diterima', DITOLAK: 'Ditolak' };
const STATUS_ORDER = [ApplicationStatus.DILAMAR, ApplicationStatus.DITINJAU, ApplicationStatus.WAWANCARA, ApplicationStatus.DITERIMA];

const ApplicationTrackerCard = ({ application, showToast }) => {
    const job = mockJobs.find(j => j.id === application.jobId);
    if (!job) return null;
    const currentStatusIndex = STATUS_ORDER.indexOf(application.status);
    const isRejected = application.status === ApplicationStatus.DITOLAK;
    const isInterview = application.status === ApplicationStatus.WAWANCARA;

    const handleAddToCalendar = () => {
        const event = { title: `Wawancara: ${job.title} di ${job.company}`, description: `Jadwal wawancara untuk posisi ${job.title}.`, location: job.company, startTime: application.interviewDate, endTime: new Date(application.interviewDate.getTime() + 60 * 60 * 1000) };
        const link = document.createElement('a');
        link.href = generateICSFile(event);
        link.download = "wawancara.ics";
        link.click();
        showToast("Jadwal ditambahkan ke kalender!", "success");
    };

    return (
        <div className="bg-white p-5 rounded-lg shadow-sm border border-slate-200 dark:bg-slate-800 dark:border-slate-700">
            <div className="flex justify-between items-start">
                <div><h4 className="font-bold text-lg text-slate-800 dark:text-slate-100">{job.title}</h4><p className="text-sm text-slate-500 dark:text-slate-400">{job.company}</p></div>
                {isRejected ? (<span className="text-xs font-bold text-white bg-red-500 px-2 py-1 rounded-full">Ditolak</span>) : (<span className="text-xs font-bold text-white bg-emerald-500 px-2 py-1 rounded-full">Aktif</span>)}
            </div>
            <div className="mt-4">
                <div className="flex justify-between items-center">{STATUS_ORDER.map((status, index) => (<div key={status} className="flex-1 text-center"><div className={`mx-auto w-8 h-8 rounded-full flex items-center justify-center border-2 ${index <= currentStatusIndex && !isRejected ? 'bg-sky-600 border-sky-600 text-white' : 'bg-gray-200 border-gray-300 text-gray-400 dark:bg-slate-700 dark:border-slate-600 dark:text-slate-500'}`}>{index < currentStatusIndex || (index === currentStatusIndex && application.status === ApplicationStatus.DITERIMA) ? <CheckCircle size={18}/> : index + 1}</div><p className={`text-xs mt-1 ${index <= currentStatusIndex && !isRejected ? 'font-bold text-sky-700 dark:text-sky-400' : 'text-slate-500 dark:text-slate-400'}`}>{status}</p></div>))}</div>
                <div className="relative w-full h-1 bg-gray-200 dark:bg-slate-700 mt-[-22px] -z-10"><div className="absolute top-0 left-0 h-1 bg-sky-600 transition-all duration-500" style={{width: `${(currentStatusIndex / (STATUS_ORDER.length -1)) * 100}%`}}></div></div>
            </div>
             {isInterview && (
                <div className="mt-4 p-3 bg-sky-50 dark:bg-sky-900/50 border-l-4 border-sky-500 rounded-r-lg">
                    <p className="font-semibold text-sky-800 dark:text-sky-300">Anda diundang untuk wawancara!</p>
                    <p className="text-sm text-sky-700 dark:text-sky-400">Jadwal: {application.interviewDate.toLocaleDateString('id-ID', { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric' })} pukul {application.interviewDate.toLocaleTimeString('id-ID', { hour: '2-digit', minute: '2-digit' })}</p>
                    <button onClick={handleAddToCalendar} className="text-sm mt-2 bg-white text-sky-600 font-semibold py-1 px-3 rounded-full border border-sky-300 hover:bg-sky-100 dark:bg-sky-800 dark:text-sky-200 dark:border-sky-700 dark:hover:bg-sky-700 flex items-center gap-2"><CalendarPlus size={14}/> Tambah ke Kalender</button>
                </div>
            )}
             <p className="text-xs text-slate-400 dark:text-slate-500 mt-4 text-center">Terakhir diperbarui: {application.lastUpdate}</p>
        </div>
    );
};

const WorkHistoryCard = ({ history }) => (
    <div className="bg-slate-50 dark:bg-slate-800 p-4 rounded-lg border border-slate-200 dark:border-slate-700">
        <div className="flex justify-between items-start">
            <div><h5 className="font-bold text-slate-800 dark:text-slate-100">{history.position}</h5><p className="text-sm text-slate-600 dark:text-slate-400">{history.company}</p><p className="text-xs text-slate-400 dark:text-slate-500 mt-1">{history.period}</p></div>
            <StarRating score={history.rating} />
        </div>
        <p className="text-sm text-slate-700 dark:text-slate-300 mt-3 italic border-l-4 border-emerald-300 dark:border-emerald-600 pl-3">"{history.comment}"</p>
    </div>
);

const SmoothLoader = () => (<div className="flex items-center justify-center h-64"><div className="relative flex"><div className="w-8 h-8 bg-emerald-600 rounded-full animate-bounce [animation-delay:-0.3s]"></div><div className="w-8 h-8 bg-emerald-600 rounded-full animate-bounce [animation-delay:-0.15s] mx-2"></div><div className="w-8 h-8 bg-emerald-600 rounded-full animate-bounce"></div></div></div>);

const LoginPage = ({ onLoginSuccess, showToast }) => {
    const [username, setUsername] = useState('');
    const [password, setPassword] = useState('');
    const handleLogin = (e) => { e.preventDefault(); if (username === 'user' && password === 'password') { localStorage.setItem('autologin', 'true'); onLoginSuccess(); showToast("Login berhasil! Selamat datang.", "success"); } else { showToast("Login gagal. Coba 'user' dan 'password'.", "error"); }};
    return (
        <div className="min-h-screen flex items-center justify-center bg-gradient-to-br from-emerald-50 to-teal-100 p-4 dark:from-slate-900 dark:to-emerald-900">
            <div className="bg-white dark:bg-slate-800 p-8 rounded-2xl shadow-xl max-w-md w-full animate-fade-in-up">
                <h1 className="text-4xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-emerald-500 to-teal-500 text-center mb-6" style={{ fontFamily: 'Poppins, sans-serif' }}>KerjaKita</h1>
                <form onSubmit={handleLogin} className="space-y-4">
                    <div className="animate-fade-in-up [animation-delay:0.2s]"><label className="block text-slate-700 dark:text-slate-300 text-sm font-medium mb-1">Username</label><input type="text" value={username} onChange={e => setUsername(e.target.value)} className="w-full px-3 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-emerald-500 dark:bg-slate-700 dark:border-slate-600 dark:text-white" placeholder="user" /></div>
                    <div className="animate-fade-in-up [animation-delay:0.3s]"><label className="block text-slate-700 dark:text-slate-300 text-sm font-medium mb-1">Password</label><input type="password" value={password} onChange={e => setPassword(e.target.value)} className="w-full px-3 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-emerald-500 dark:bg-slate-700 dark:border-slate-600 dark:text-white" placeholder="password" /></div>
                    <button type="submit" className="w-full bg-gradient-to-r from-emerald-500 to-teal-600 text-white font-bold py-3 rounded-lg hover:from-emerald-600 hover:to-teal-700 transition transform hover:scale-105 animate-fade-in-up [animation-delay:0.4s]">Masuk</button>
                </form>
            </div>
        </div>
    );
};

const HomePage = ({ setActiveTab, openJobModal, recommendedJobs, popularJobs }) => ( <div className="space-y-10"><section><h2 className="text-3xl font-bold text-slate-800 dark:text-slate-100 mb-1" style={{ fontFamily: 'Poppins, sans-serif' }}>Rekomendasi Untuk Anda</h2><p className="text-slate-600 dark:text-slate-400 mb-4">Pekerjaan yang kami pilih berdasarkan minat Anda.</p><div className="grid grid-cols-1 md:grid-cols-2 gap-6">{recommendedJobs.map(job => <JobCard key={job.id} job={job} onClick={() => openJobModal(job)} />)}</div></section><section><h3 className="text-2xl font-bold text-slate-800 dark:text-slate-100 mb-4 flex items-center"><TrendingUp className="mr-3 text-sky-600" /> Sedang Populer</h3><div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">{popularJobs.map(job => <JobCard key={job.id} job={job} onClick={() => openJobModal(job)} isCompact={true} />)}</div><button onClick={() => setActiveTab('jobs')} className="mt-6 text-sky-600 dark:text-sky-400 font-semibold hover:underline flex items-center">Lihat Semua Pekerjaan <ChevronRight className="ml-1" size={20} /></button></section></div>);
const JobsPage = ({ jobs, filters, dispatch, openJobModal }) => ( <><h2 className="text-3xl font-bold text-slate-800 dark:text-slate-100" style={{ fontFamily: 'Poppins, sans-serif' }}>Cari Pekerjaan Layak</h2><p className="text-slate-600 dark:text-slate-400 mb-6">Gunakan filter dan skor kami untuk menemukan pekerjaan yang tepat.</p><div className="bg-white dark:bg-slate-800 p-4 rounded-lg shadow-md mb-6"><div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4"><div className="relative col-span-1 lg:col-span-2"><Search className="absolute left-3 top-1/2 -translate-y-1/2 text-gray-400" size={20} /><input type="text" placeholder="Cari pekerjaan..." className="w-full pl-10 pr-4 py-2 border border-gray-300 rounded-lg dark:bg-slate-700 dark:border-slate-600 dark:text-white" value={filters.searchTerm} onChange={e => dispatch({ type: 'SET_FILTER', payload: { key: 'searchTerm', value: e.target.value } })} /></div><select className="w-full py-2 px-3 border border-gray-300 rounded-lg bg-white dark:bg-slate-700 dark:border-slate-600 dark:text-white" value={filters.jobTypeFilter} onChange={e => dispatch({ type: 'SET_FILTER', payload: { key: 'jobTypeFilter', value: e.target.value } })}><option value="">Semua Tipe</option><option value="Full-time">Full-time</option><option value="Part-time">Part-time</option><option value="Freelance">Freelance</option></select><select className="w-full py-2 px-3 border border-gray-300 rounded-lg bg-white dark:bg-slate-700 dark:border-slate-600 dark:text-white" value={filters.sortBy} onChange={e => dispatch({ type: 'SET_FILTER', payload: { key: 'sortBy', value: e.target.value } })}><option value="relevance">Urutkan: Relevansi</option><option value="score">Urutkan: Skor Tertinggi</option></select><div className="col-span-full flex items-center justify-center bg-slate-50 dark:bg-slate-700/50 p-2 rounded-lg"><input type="checkbox" id="decentWorkFilter" className="form-checkbox h-5 w-5 text-emerald-600 rounded focus:ring-emerald-500" checked={filters.showDecentWorkOnly} onChange={e => dispatch({ type: 'SET_FILTER', payload: { key: 'showDecentWorkOnly', value: e.target.checked } })} /><label htmlFor="decentWorkFilter" className="ml-2 text-slate-700 dark:text-slate-300 cursor-pointer">Hanya Pekerjaan Terverifikasi</label></div></div></div><div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">{jobs.length > 0 ? jobs.map(job => <JobCard key={job.id} job={job} onClick={() => openJobModal(job)} />) : <p className="col-span-full text-center text-slate-500">Tidak ada pekerjaan yang cocok dengan filter Anda.</p>}</div></> );
const LearnPage = ({ courses, filters, dispatch, onSave, showToast }) => ( <><h2 className="text-3xl font-bold text-slate-800 dark:text-slate-100 mb-6" style={{fontFamily: 'Poppins, sans-serif'}}>Tingkatkan Keterampilan</h2><div className="bg-white dark:bg-slate-800 p-4 rounded-lg shadow-md mb-6"><div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4"><div className="relative col-span-full lg:col-span-2"><Search className="absolute left-3 top-1/2 -translate-y-1/2 text-gray-400" size={20} /><input type="text" placeholder="Cari kursus..." className="w-full pl-10 pr-4 py-2 border rounded-lg dark:bg-slate-700 dark:border-slate-600 dark:text-white" value={filters.searchTerm} onChange={e => dispatch({type:'SET_FILTER', payload:{key:'searchTerm', value:e.target.value}})} /></div><select className="w-full py-2 px-3 border rounded-lg bg-white dark:bg-slate-700 dark:border-slate-600 dark:text-white" value={filters.courseCategoryFilter} onChange={e => dispatch({type:'SET_FILTER', payload:{key:'courseCategoryFilter', value:e.target.value}})}><option value="">Semua Kategori</option><option value="Pemasaran">Pemasaran</option><option value="Teknologi">Teknologi</option><option value="Produk">Produk</option><option value="Desain">Desain</option></select><select className="w-full py-2 px-3 border rounded-lg bg-white dark:bg-slate-700 dark:border-slate-600 dark:text-white" value={filters.coursePriceFilter} onChange={e => dispatch({type:'SET_FILTER', payload:{key:'coursePriceFilter', value:e.target.value}})}><option value="">Semua Harga</option><option value="Gratis">Gratis</option><option value="Berbayar">Berbayar</option></select></div></div><div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">{courses.length > 0 ? courses.map(course => <CourseCard key={course.id} course={course} onSave={onSave} showToast={showToast} />) : <p className="col-span-full text-center text-slate-500 dark:text-slate-400">Tidak ada kursus yang cocok.</p>}</div></> );
const SupportPage = ({ umkm, filters, dispatch, showToast, apiKey }) => {
    const [keywords, setKeywords] = useState('');
    const [ideas, setIdeas] = useState('');
    const [isLoading, setIsLoading] = useState(false);
    const generateIdeas = async () => { if (!keywords.trim()) return showToast("Mohon masukkan kata kunci.", "error"); setIsLoading(true); const p = `Hasilkan 3 ide bisnis UMKM inovatif di Indonesia berdasarkan kata kunci: "${keywords}". Berikan nama, deskripsi singkat, dan alasan keberlanjutannya.`; const res = await callGeminiAPI(p, apiKey); setIdeas(res); setIsLoading(false); };
    return <><h2 className="text-3xl font-bold text-slate-800 dark:text-slate-100 mb-6" style={{fontFamily: 'Poppins, sans-serif'}}>Dukung UMKM Lokal</h2><div className="bg-white dark:bg-slate-800 p-4 rounded-lg shadow-md mb-6 flex flex-col md:flex-row gap-4"><div className="relative flex-grow"><Search className="absolute left-3 top-1/2 -translate-y-1/2 text-gray-400" size={20} /><input type="text" placeholder="Cari UMKM..." className="w-full pl-10 pr-4 py-2 border rounded-lg dark:bg-slate-700 dark:border-slate-600 dark:text-white" value={filters.searchTerm} onChange={e => dispatch({type:'SET_FILTER', payload:{key:'searchTerm', value:e.target.value}})} /></div><div className="flex items-center justify-center p-2 rounded-lg bg-slate-50 dark:bg-slate-700/50 flex-shrink-0"><input type="checkbox" id="umkmSustainableFilter" className="form-checkbox h-5 w-5 text-violet-600 rounded focus:ring-violet-500" checked={filters.umkmSustainableOnly} onChange={e => dispatch({type:'SET_FILTER', payload:{key:'umkmSustainableOnly', value:e.target.checked}})} /><label htmlFor="umkmSustainableFilter" className="ml-2 text-slate-700 dark:text-slate-300 cursor-pointer">Hanya Berkelanjutan</label></div></div><div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">{umkm.length > 0 ? umkm.map(u => <UmkmCard key={u.id} umkm={u} showToast={showToast} />) : <p className="col-span-full text-center text-slate-500 dark:text-slate-400">Tidak ada UMKM yang cocok.</p>}</div><section className="bg-gradient-to-br from-violet-100 to-pink-100 dark:from-violet-900/30 dark:to-pink-900/30 p-6 rounded-lg shadow-md mt-8"><h3 className="text-2xl font-bold text-slate-800 dark:text-slate-100 mb-2">Generator Ide Bisnis ✨</h3><p className="text-slate-700 dark:text-slate-300 mb-4">Butuh inspirasi? Biarkan AI membantu!</p><textarea className="w-full p-3 border rounded-lg mb-4 dark:bg-slate-800 dark:border-slate-600 dark:text-white" rows="3" placeholder="Contoh: daur ulang, makanan sehat..." value={keywords} onChange={e => setKeywords(e.target.value)} /><button onClick={generateIdeas} className="bg-violet-600 text-white font-semibold py-2 px-4 rounded-lg hover:bg-violet-700" disabled={isLoading}>{isLoading ? 'Menghasilkan...' : 'Hasilkan Ide'}</button>{ideas && <div className="mt-6 bg-white dark:bg-slate-800 p-4 rounded-lg"><h4 className="font-bold mb-2 dark:text-slate-200">Ide Bisnis:</h4><p className="text-slate-700 dark:text-slate-300 whitespace-pre-wrap">{ideas}</p></div>}</section></>;
};
const ProfilePage = ({ onLogout, savedItems, appliedJobs, openJobModal, setPage }) => {
    return (<div className="grid grid-cols-1 lg:grid-cols-3 gap-8"><div className="lg:col-span-1 space-y-8"><div className="bg-white dark:bg-slate-800 p-6 rounded-lg shadow-md text-center"><img src={userProfile.avatar} alt="User Avatar" className="w-24 h-24 rounded-full object-cover mx-auto mb-4 border-4 border-white dark:border-slate-700 shadow-md"/><p className="font-semibold text-xl dark:text-white">{userProfile.name}</p><p className="text-sm text-slate-500 dark:text-slate-400">{userProfile.email}</p><button onClick={onLogout} className="mt-6 w-full bg-red-500 text-white font-semibold py-2 rounded-lg hover:bg-red-600 transition">Keluar</button></div><div className="bg-white dark:bg-slate-800 p-6 rounded-lg shadow-md"><h3 className="font-bold mb-4 text-lg dark:text-slate-100">Pengaturan & Info</h3><div className="space-y-1">{[{label:'Pengaturan', icon:Settings, page:'settings'}, {label:'Tentang Kami', icon:Building, page:'about'}, {label:'Syarat & Kebijakan', icon:FileBadge2, page:'terms'}].map(item => (<button key={item.page} onClick={() => setPage(item.page)} className="w-full flex items-center gap-3 p-2 rounded-md text-slate-600 dark:text-slate-300 hover:bg-slate-100 dark:hover:bg-slate-700"><item.icon size={20}/><span>{item.label}</span></button>))}</div></div></div><div className="lg:col-span-2 space-y-8"><div className="bg-white dark:bg-slate-800 p-6 rounded-lg shadow-md"><h3 className="text-xl font-bold text-slate-800 dark:text-slate-100 mb-4 flex items-center"><Briefcase className="mr-2 text-sky-600" />Status Lamaran Saya</h3><div className="space-y-4">{appliedJobs.length > 0 ? (appliedJobs.map(app => <ApplicationTrackerCard key={app.jobId} application={app} showToast={() => {}} />)) : (<p className="text-center text-slate-500 dark:text-slate-400 py-4">Anda belum melamar pekerjaan.</p>)}</div></div><div className="bg-white dark:bg-slate-800 p-6 rounded-lg shadow-md"><h3 className="text-xl font-bold text-slate-800 dark:text-slate-100 mb-4 flex items-center"><Award className="mr-2 text-amber-500" />Riwayat & Reputasi Kerja</h3><div className="space-y-4">{userProfile.workHistory.map((history, index) => (<WorkHistoryCard key={index} history={history} />))}</div></div></div></div>);
};
const SettingsPage = ({ setPage, theme, setTheme }) => (
    <div className="max-w-4xl mx-auto">
        <button onClick={() => setPage('profile')} className="flex items-center gap-2 text-slate-500 dark:text-slate-400 hover:text-emerald-600 dark:hover:text-emerald-400 mb-6"><ChevronLeft size={20}/> Kembali ke Profil</button>
        <h2 className="text-3xl font-bold text-slate-800 dark:text-slate-100 mb-6">Pengaturan</h2>
        <div className="bg-white dark:bg-slate-800 p-6 rounded-lg shadow-md space-y-6">
            <div><h3 className="text-lg font-semibold text-slate-700 dark:text-slate-200">Notifikasi</h3><div className="mt-2 space-y-2"><div className="flex justify-between items-center"><p className="dark:text-slate-300">Notifikasi lamaran kerja</p><label className="switch"><input type="checkbox" defaultChecked/><span className="slider round"></span></label></div><div className="flex justify-between items-center"><p className="dark:text-slate-300">Rekomendasi pekerjaan</p><label className="switch"><input type="checkbox" defaultChecked/><span className="slider round"></span></label></div></div></div>
            <div className="border-t dark:border-slate-700 pt-6"><h3 className="text-lg font-semibold text-slate-700 dark:text-slate-200">Tema Tampilan</h3><div className="mt-2 flex gap-4"><button onClick={() => setTheme('light')} className={`flex items-center gap-2 p-2 rounded-md border-2 ${theme === 'light' ? 'border-emerald-500 bg-emerald-50' : 'border-gray-300 dark:border-slate-600'}`}><Sun/> Terang</button><button onClick={() => setTheme('dark')} className={`flex items-center gap-2 p-2 rounded-md border-2 ${theme === 'dark' ? 'border-emerald-500 bg-slate-700' : 'border-gray-300 dark:border-slate-600'}`}><Moon/> Gelap</button></div></div>
        </div>
    </div>
);
const AboutUsPage = ({ setPage }) => ( <div className="max-w-4xl mx-auto"><button onClick={() => setPage('profile')} className="flex items-center gap-2 text-slate-500 dark:text-slate-400 hover:text-emerald-600 dark:hover:text-emerald-400 mb-6"><ChevronLeft size={20}/> Kembali ke Profil</button><div className="bg-white dark:bg-slate-800 p-8 rounded-lg shadow-md"><h2 className="text-3xl font-bold text-transparent bg-clip-text bg-gradient-to-r from-emerald-500 to-teal-500 mb-4">Tentang KerjaKita</h2><p className="text-slate-600 dark:text-slate-300 leading-relaxed">Misi kami adalah menciptakan ekosistem karir yang adil, transparan, dan mendukung pertumbuhan bagi setiap individu di Indonesia. Kami percaya bahwa pekerjaan yang layak bukan hanya tentang gaji, tetapi tentang lingkungan kerja yang sehat, kesempatan berkembang, dan kesejahteraan. Melalui teknologi, kami menghubungkan talenta dengan peluang terbaik yang sesuai dengan nilai-nilai mereka.</p></div></div>);
const TermsPage = ({ setPage }) => ( <div className="max-w-4xl mx-auto"><button onClick={() => setPage('profile')} className="flex items-center gap-2 text-slate-500 dark:text-slate-400 hover:text-emerald-600 dark:hover:text-emerald-400 mb-6"><ChevronLeft size={20}/> Kembali ke Profil</button><div className="bg-white dark:bg-slate-800 p-8 rounded-lg shadow-md"><h2 className="text-3xl font-bold text-slate-800 dark:text-slate-100 mb-4">Syarat & Kebijakan</h2><p className="text-slate-600 dark:text-slate-300">Dengan menggunakan aplikasi ini, Anda setuju untuk mematuhi semua syarat dan ketentuan yang berlaku...</p></div></div>);

const JobCard = React.memo(function JobCard({ job, onClick, isCompact = false }) { const score = useMemo(() => calculateDecentWorkScore(job.decentWorkCriteria), [job.decentWorkCriteria]); if (isCompact) { return <div onClick={onClick} className="bg-white dark:bg-slate-800 rounded-lg shadow-sm border dark:border-slate-700 hover:shadow-lg dark:hover:border-emerald-500 transition-shadow cursor-pointer p-4 flex items-center gap-4"><img src={job.companyLogo} onError={(e) => { e.target.onerror = null; e.target.src="https://placehold.co/100x100/cccccc/333333?text=Logo"; }} alt={`${job.company} logo`} className="w-16 h-16 object-contain rounded-md flex-shrink-0 bg-slate-50 dark:bg-slate-700" /><div className="flex-grow overflow-hidden"><h4 className="font-bold text-slate-800 dark:text-slate-100 truncate">{job.title}</h4><p className="text-sm text-slate-500 dark:text-slate-400 truncate">{job.company}</p><StarRating score={score} size={14} className="mt-1" /></div></div>; } return <div onClick={onClick} className="bg-white dark:bg-slate-800 rounded-lg shadow-md border dark:border-slate-700 hover:shadow-xl hover:border-emerald-600 dark:hover:border-emerald-500 transition-all cursor-pointer flex flex-col overflow-hidden transform hover:-translate-y-1"><img src={job.image} alt={job.title} className="w-full h-40 object-cover"/><div className="p-5 flex flex-col flex-grow"><div><h3 className="text-lg font-bold text-slate-800 dark:text-slate-100" style={{ fontFamily: 'Poppins, sans-serif' }}>{job.title}</h3><p className="text-sm text-sky-700 dark:text-sky-400 font-medium mb-2">{job.company}</p><div className="flex items-center gap-2 mb-3"><StarRating score={score} /><span className="text-xs text-slate-500 dark:text-slate-400 font-semibold">{score.toFixed(1)}/5.0</span></div></div><div className="mt-auto pt-3 border-t border-gray-100 dark:border-slate-700 flex items-center justify-between text-sm"><span className="flex items-center gap-1 text-slate-600 dark:text-slate-400"><MapPin size={14} />{job.location}</span><span className="font-semibold text-emerald-600 dark:text-emerald-400">{job.salary.split(' - ')[0]}</span></div></div></div>; });
const CourseCard = React.memo(function CourseCard({ course, onSave, showToast }) { 
    const handleAddToCalendar = () => {
        const nextDay = (dayName) => { const days = ['minggu', 'senin', 'selasa', 'rabu', 'kamis', 'jumat', 'sabtu']; const targetDay = days.indexOf(dayName.toLowerCase()); const today = new Date(); today.setDate(today.getDate() + (targetDay + 7 - today.getDay()) % 7); return today; };
        const [hour, minute] = course.schedule.time.split(':');
        const eventDate = nextDay(course.schedule.day);
        eventDate.setHours(parseInt(hour), parseInt(minute), 0, 0);
        const event = { title: `Pelatihan: ${course.title}`, description: `Jadwal untuk pelatihan ${course.title} oleh ${course.provider}.`, location: course.provider, startTime: eventDate, endTime: new Date(eventDate.getTime() + 90 * 60 * 1000) };
        const icsUri = generateICSFile(event);
        const link = document.createElement('a');
        link.href = icsUri;
        link.download = "pelatihan.ics";
        link.click();
        showToast("Jadwal pelatihan ditambahkan!", "success");
    };
    return <div className="bg-white dark:bg-slate-800 rounded-lg shadow-md border dark:border-slate-700 flex flex-col overflow-hidden"><img src={course.image} alt={course.title} className="w-full h-40 object-cover"/><div className="p-5 flex flex-col flex-grow"><h3 className="font-bold text-lg dark:text-slate-100">{course.title}</h3><p className="text-sm text-slate-600 dark:text-slate-400 mb-2">{course.provider}</p><p className="text-xs text-sky-600 bg-sky-50 dark:text-sky-300 dark:bg-sky-900/50 font-semibold px-2 py-1 rounded-full w-fit">Jadwal: Setiap {course.schedule.day}, {course.schedule.time}</p><div className="mt-auto flex gap-2 pt-4"><button onClick={handleAddToCalendar} className="flex-1 text-center bg-sky-500 text-white font-semibold py-2 px-4 rounded-lg hover:bg-sky-600 flex items-center justify-center gap-2"><CalendarPlus size={16}/> Kalender</button><button onClick={() => { onSave(course); showToast(`Kursus "${course.title}" disimpan!`, 'success'); }} className="bg-gray-200 dark:bg-slate-700 p-2 rounded-lg hover:bg-gray-300 dark:hover:bg-slate-600"><Heart className="dark:text-slate-300" size={20} /></button></div></div></div> 
});
const UmkmCard = React.memo(function UmkmCard({ umkm, showToast }) { return <div className="bg-white dark:bg-slate-800 rounded-lg shadow-md border dark:border-slate-700 hover:shadow-lg transition-shadow flex flex-col overflow-hidden"><img src={umkm.image} alt={umkm.name} className="w-full h-40 object-cover" /><div className="p-5 flex flex-col flex-grow"><h3 className="font-bold text-lg dark:text-slate-100">{umkm.name}</h3><p className="text-sm text-violet-600 dark:text-violet-400 font-medium">{umkm.category}</p><div className="flex items-center gap-2 my-2"><StarRating score={umkm.rating} /><span className="text-xs text-slate-500 dark:text-slate-400">({umkm.reviews} ulasan)</span></div><button onClick={() => showToast(`Terima kasih telah mendukung ${umkm.name}!`, 'success')} className="mt-auto w-full bg-violet-600 text-white font-semibold py-2 px-4 rounded-lg hover:bg-violet-700">Dukung Sekarang</button></div></div> });
const NavItem = React.memo(function NavItem({ icon: Icon, label, active, onClick }) { return <button className={`flex flex-col items-center justify-center flex-grow text-sm transition-colors ${active ? 'text-emerald-600 dark:text-emerald-400' : 'text-slate-500 dark:text-slate-400 hover:text-emerald-600 dark:hover:text-emerald-500'}`} onClick={onClick}><Icon size={24} className="mb-1" /><span>{label}</span></button> });
const JobDetailModal = ({ job, isOpen, onClose, showToast, onSave, onApply, apiKey }) => {
    const [coverLetter, setCoverLetter] = useState('');
    const [isLoadingCL, setIsLoadingCL] = useState(false);
    const generateCoverLetter = async () => { setIsLoadingCL(true); setCoverLetter(''); const p = `Buat draf surat lamaran singkat dan profesional untuk ${userProfile.name} yang melamar sebagai ${job.title} di ${job.company}. Tonjolkan kesesuaian minat (${userProfile.interests.join(', ')}) dengan deskripsi: ${job.description}.`; const result = await callGeminiAPI(p, apiKey); setCoverLetter(result); setIsLoadingCL(false); };
    if (!isOpen || !job) return null; 
    const score = calculateDecentWorkScore(job.decentWorkCriteria); 
    const criteria = job.decentWorkCriteria || {}; 
    return ( <div className="fixed inset-0 bg-black bg-opacity-60 flex items-center justify-center p-4 z-50 animate-fade-in" onClick={onClose}><div className="bg-white dark:bg-slate-800 rounded-xl shadow-xl max-w-2xl w-full max-h-[90vh] flex flex-col" onClick={e => e.stopPropagation()}><header className="p-4 border-b dark:border-slate-700 flex justify-between items-center"><h2 className="text-xl font-bold dark:text-slate-100">{job.title}</h2><button onClick={onClose} className="p-1 rounded-full dark:text-slate-300"><X size={24} /></button></header><div className="p-6 overflow-y-auto space-y-6"><div className="bg-sky-50 dark:bg-sky-900/50 border border-sky-200 dark:border-sky-800 p-4 rounded-lg"><h3 className="text-lg font-bold text-sky-800 dark:text-sky-300 mb-3 flex items-center"><Award size={20} className="mr-2" />Skor Pekerjaan Layak</h3><div className="flex items-center mb-4"><StarRating score={score} size={24} /><span className="text-2xl font-bold text-sky-700 dark:text-sky-300 ml-3">{score.toFixed(1)}</span><span className="text-slate-500 dark:text-slate-400 ml-1">/ 5.0</span></div><div className="grid grid-cols-1 sm:grid-cols-2 gap-x-4 gap-y-2 text-sm text-slate-600 dark:text-slate-300"><div className="flex items-center justify-between"><span>Gaji & Transparansi</span> <StarRating score={criteria.salary || 0} /></div><div className="flex items-center justify-between"><span>Tunjangan & Jaminan</span> <StarRating score={criteria.benefits || 0} /></div><div className="flex items-center justify-between"><span>Kejelasan Informasi</span> <StarRating score={criteria.transparency || 0} /></div><div className="flex items-center justify-between"><span>Peluang Karir</span> <StarRating score={criteria.development || 0} /></div></div></div><p className="dark:text-slate-300">{job.description}</p><div><h3 className="font-semibold dark:text-slate-200">Persyaratan & Manfaat...</h3></div><div className="border-t dark:border-slate-700 pt-6"><h3 className="text-lg font-bold text-slate-800 dark:text-slate-100 mb-2 flex items-center"><Sparkles className="mr-2 text-sky-600" />Asisten Surat Lamaran</h3><p className="text-sm text-slate-600 dark:text-slate-400 mb-4">Biarkan AI membuatkan draf surat lamaran untuk Anda.</p><button onClick={generateCoverLetter} className="bg-sky-100 text-sky-700 font-semibold py-2 px-4 rounded-lg hover:bg-sky-200 transition dark:bg-sky-900/80 dark:text-sky-300 dark:hover:bg-sky-900" disabled={isLoadingCL}>{isLoadingCL ? 'Membuat draf...' : 'Buat Draf Surat Lamaran ✨'}</button>{coverLetter && <div className="mt-4 bg-slate-50 dark:bg-slate-700/50 p-4 rounded-lg border dark:border-slate-600"><h4 className="font-semibold mb-2 dark:text-slate-200">Draf Surat Lamaran:</h4><p className="text-slate-700 dark:text-slate-300 whitespace-pre-wrap text-sm">{coverLetter}</p></div>}</div></div><footer className="p-4 border-t dark:border-slate-700 flex justify-end gap-3 bg-slate-50 dark:bg-slate-800/50"><button onClick={() => { onSave(job); showToast('Pekerjaan disimpan!', 'success'); }} className="bg-gray-200 dark:bg-slate-700 dark:text-slate-200 font-semibold py-2 px-4 rounded-lg">Simpan</button><button onClick={() => {onApply(job); onClose();}} className="bg-emerald-600 text-white font-bold py-2 px-6 rounded-lg">Lamar Sekarang</button></footer></div></div> );
};

// ===================================================================================
// 5. MAIN APP COMPONENT
// ===================================================================================

function App() {
    const [isLoggedIn, setIsLoggedIn] = useState(false);
    const [isLoading, setIsLoading] = useState(true);
    const [selectedJob, setSelectedJob] = useState(null);
    const [isJobModalOpen, setIsJobModalOpen] = useState(false);
    const [toast, showToast] = useToast();
    const [filters, dispatchFilters] = useReducer(filterReducer, initialFilterState);
    const [savedItems, setSavedItems] = useState({ jobs: [], courses: [] });
    const [appliedJobs, setAppliedJobs] = useState([]);
    const [theme, setTheme] = useState('light');
    const [page, setPage] = useState('home');
    const apiKey = ""; // API key is optional here

    useEffect(() => { if (localStorage.getItem('autologin') === 'true') setIsLoggedIn(true); setIsLoading(false); }, []);
    useEffect(() => { 
        const root = window.document.documentElement;
        root.classList.remove(theme === 'dark' ? 'light' : 'dark');
        root.classList.add(theme);
        localStorage.setItem('theme', theme);
    }, [theme]);
    
    useEffect(() => { 
        if (isLoggedIn && savedItems.jobs.length === 0) {
            setSavedItems({ jobs: mockJobs.filter(j => userProfile.savedJobIds.includes(j.id)), courses: mockCourses.filter(c => userProfile.savedCourseIds.includes(c.id)) });
            setAppliedJobs([
                { jobId: 'j1', status: ApplicationStatus.WAWANCARA, lastUpdate: 'Kemarin', interviewDate: new Date('2025-06-10T14:00:00') },
                { jobId: 'j7', status: ApplicationStatus.DITOLAK, lastUpdate: '3 hari lalu' }
            ]);
        }
    }, [isLoggedIn, savedItems.jobs.length]);

    useEffect(() => { 
        if (!isLoggedIn) return; 
        setIsLoading(true); 
        const t = setTimeout(() => setIsLoading(false), 300); 
        return () => clearTimeout(t); 
    }, [page, isLoggedIn]);
    
    const handleLoginSuccess = useCallback(() => setIsLoggedIn(true), []);
    const handleLogout = useCallback(() => { setIsLoggedIn(false); localStorage.removeItem('autologin'); setSavedItems({jobs: [], courses: []}); setAppliedJobs([]); setPage('home'); showToast("Anda telah keluar.", "info"); }, [showToast]);
    const handleSaveItem = useCallback((item, type) => { setSavedItems(prev => prev[type].some(s => s.id === item.id) ? prev : { ...prev, [type]: [...prev[type], item] }); }, []);
    const handleApplyJob = useCallback((job) => {
        setAppliedJobs(prev => {
            if (prev.some(app => app.jobId === job.id)) {
                showToast("Anda sudah melamar pekerjaan ini.", "info");
                return prev;
            }
            showToast("Lamaran Anda berhasil dikirim!", "success");
            const newApplication = { jobId: job.id, status: ApplicationStatus.DILAMAR, lastUpdate: 'Baru saja' };
            return [newApplication, ...prev];
        });
    }, [showToast]);

    const openJobModal = useCallback(job => { setSelectedJob(job); setIsJobModalOpen(true); }, []);
    const closeJobModal = useCallback(() => { setSelectedJob(null); setIsJobModalOpen(false); }, []);
    const changeTab = useCallback(tabName => { setPage(tabName); dispatchFilters({ type: 'RESET_FILTERS' }); }, []);
    
    const recommendedJobs = useMemo(() => mockJobs.filter(job => userProfile.interests.includes(job.category)).slice(0, 2), []);
    const popularJobs = useMemo(() => [...mockJobs].sort((a,b) => calculateDecentWorkScore(b.decentWorkCriteria) - calculateDecentWorkScore(a.decentWorkCriteria)).slice(0, 3), []);
    const filteredAndSortedJobs = useMemo(() => { let j = mockJobs.filter(job => (job.title.toLowerCase().includes(filters.searchTerm.toLowerCase()) || job.company.toLowerCase().includes(filters.searchTerm.toLowerCase())) && (!filters.showDecentWorkOnly || job.isDecentWork) && (filters.jobTypeFilter === '' || job.jobType === filters.jobTypeFilter)); if (filters.sortBy === 'score') j.sort((a, b) => calculateDecentWorkScore(b.decentWorkCriteria) - calculateDecentWorkScore(a.decentWorkCriteria)); return j; }, [filters]);
    const filteredCourses = useMemo(() => mockCourses.filter(c => (filters.courseCategoryFilter === '' || c.category === filters.courseCategoryFilter) && (filters.coursePriceFilter === '' || (filters.coursePriceFilter === 'Gratis' && !c.isPaid) || (filters.coursePriceFilter === 'Berbayar' && c.isPaid)) && c.title.toLowerCase().includes(filters.searchTerm.toLowerCase())), [filters]);
    const filteredUmkm = useMemo(() => mockUmkm.filter(u => (!filters.umkmSustainableOnly || u.isSustainable) && u.name.toLowerCase().includes(filters.searchTerm.toLowerCase())), [filters]);

    if (isLoading && !isLoggedIn) return <div className="min-h-screen bg-slate-50 dark:bg-slate-900"><SmoothLoader /></div>;
    if (!isLoggedIn) return <div className={`min-h-screen bg-slate-50 ${theme}`}><FontImports /><LoginPage onLoginSuccess={handleLoginSuccess} showToast={showToast} /><Toast {...toast} /></div>;
    
    const renderContent = () => {
        if (isLoading) return <SmoothLoader />;
        switch (page) {
            case 'home': return <HomePage setActiveTab={changeTab} openJobModal={openJobModal} recommendedJobs={recommendedJobs} popularJobs={popularJobs} />;
            case 'jobs': return <JobsPage jobs={filteredAndSortedJobs} filters={filters} dispatch={dispatchFilters} openJobModal={openJobModal} />;
            case 'learn': return <LearnPage courses={filteredCourses} filters={filters} dispatch={dispatchFilters} onSave={item => handleSaveItem(item, 'courses')} showToast={showToast} />;
            case 'support': return <SupportPage umkm={filteredUmkm} filters={filters} dispatch={dispatchFilters} showToast={showToast} apiKey={apiKey} />;
            case 'profile': return <ProfilePage onLogout={handleLogout} savedItems={savedItems} appliedJobs={appliedJobs} openJobModal={openJobModal} setPage={setPage} />;
            case 'settings': return <SettingsPage setPage={setPage} theme={theme} setTheme={setTheme} />;
            case 'about': return <AboutUsPage setPage={setPage} />;
            case 'terms': return <TermsPage setPage={setPage} />;
            default: return <HomePage setActiveTab={changeTab} openJobModal={openJobModal} recommendedJobs={recommendedJobs} popularJobs={popularJobs} />;
        }
    };

    return (
        <div className="min-h-screen bg-slate-50 dark:bg-slate-900 flex flex-col" style={{ fontFamily: 'Inter, sans-serif' }}>
            <style>{`.animate-fade-in { animation: fadeIn 0.5s ease-in-out; } @keyframes fadeIn { from { opacity: 0; transform: translateY(10px); } to { opacity: 1; transform: translateY(0); } } .animate-fade-in-up { animation: fadeInUp 0.5s ease-in-out forwards; opacity: 0; } @keyframes fadeInUp { from { opacity: 0; transform: translateY(20px); } to { opacity: 1; transform: translateY(0); } } .switch { position: relative; display: inline-block; width: 44px; height: 24px; } .switch input { opacity: 0; width: 0; height: 0; } .slider { position: absolute; cursor: pointer; top: 0; left: 0; right: 0; bottom: 0; background-color: #ccc; transition: .4s; } .slider:before { position: absolute; content: ""; height: 16px; width: 16px; left: 4px; bottom: 4px; background-color: white; transition: .4s; } input:checked + .slider { background-color: #10b981; } input:focus + .slider { box-shadow: 0 0 1px #10b981; } input:checked + .slider:before { transform: translateX(20px); } .slider.round { border-radius: 34px; } .slider.round:before { border-radius: 50%; }`}</style>
            <FontImports />
            <header className="bg-white/80 dark:bg-slate-900/80 backdrop-blur-sm shadow-sm p-4 flex items-center justify-between sticky top-0 z-30">
                <h1 className="text-3xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-emerald-500 to-teal-500" style={{ fontFamily: 'Poppins, sans-serif' }}>KerjaKita</h1>
                <button onClick={handleLogout} className="text-gray-500 hover:text-red-500 p-2 rounded-full hidden sm:block"><LogOut size={24} /></button>
            </header>
            <main className="flex-grow overflow-y-auto p-4 sm:p-6 pb-24">{renderContent()}</main>
            <nav className="fixed bottom-0 left-0 right-0 bg-white/80 dark:bg-slate-900/80 backdrop-blur-sm border-t dark:border-slate-700 z-40">
                <div className="flex justify-around h-16 max-w-4xl mx-auto">
                    <NavItem icon={Home} label="Beranda" active={page === 'home'} onClick={() => changeTab('home')} />
                    <NavItem icon={Briefcase} label="Pekerjaan" active={page === 'jobs'} onClick={() => changeTab('jobs')} />
                    <NavItem icon={BookOpen} label="Belajar" active={page === 'learn'} onClick={() => changeTab('learn')} />
                    <NavItem icon={Handshake} label="Dukung" active={page === 'support'} onClick={() => changeTab('support')} />
                    <NavItem icon={User} label="Profil" active={['profile', 'settings', 'about', 'terms'].includes(page)} onClick={() => changeTab('profile')} />
                </div>
            </nav>
            <JobDetailModal isOpen={isJobModalOpen} job={selectedJob} onClose={closeJobModal} showToast={showToast} onSave={(item) => handleSaveItem(item, 'jobs')} onApply={handleApplyJob} apiKey={apiKey} />
            <Toast {...toast} />
        </div>
    );
}

export default App;
