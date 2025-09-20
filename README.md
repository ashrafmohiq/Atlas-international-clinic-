# Atlas-international-clinic-
Medical and dental clinics
export default function HomePage() { return ( <div className="bg-white text-gray-800"> {/* Header */} <header className="flex justify-between items-center p-4 shadow-md bg-blue-600 text-white"> <h1 className="text-xl font-bold">عيادات أطلس الدولية</h1> <nav className="space-x-4 hidden md:flex"> <a href="#about" className="hover:underline">من نحن</a> <a href="#services" className="hover:underline">الخدمات</a> <a href="#blog" className="hover:underline">المقالات</a> <a href="#contact" className="hover:underline">اتصل بنا</a> </nav> <button className="bg-white text-blue-600 px-4 py-2 rounded-xl font-semibold">احجز الآن</button> </header>

{/* Hero Section */}
  <section className="flex flex-col items-center text-center py-16 bg-blue-50">
    <h2 className="text-3xl font-bold text-blue-700 mb-4">
      عيادات أطلس الدولية – د. أشرف محمد العراقي
    </h2>
    <p className="text-lg max-w-2xl mb-6">
      خبرة في زراعة، تقويم، وتجميل الأسنان مع خدمات طبية متكاملة بأحدث الأجهزة.
    </p>
    <div className="space-x-4">
      <button className="bg-blue-600 text-white px-6 py-3 rounded-2xl shadow">احجز موعدك الآن</button>
      <button className="bg-gray-200 text-gray-800 px-6 py-3 rounded-2xl shadow">اتصل بنا</button>
    </div>
  </section>

  {/* About Section */}
  <section id="about" className="py-16 px-6 md:px-20 bg-white">
    <h3 className="text-2xl font-bold text-blue-700 mb-4">من نحن</h3>
    <p className="text-lg leading-relaxed">
      أنا د. أشرف محمد العراقي – أخصائي زراعة وتقويم وتجميل الأسنان. أسست مركز عيادات أطلس الدولية ليكون وجهة متكاملة للرعاية الطبية المتخصصة في الإسكندرية.
    </p>
  </section>

  {/* Services Section */}
  <section id="services" className="py-16 px-6 md:px-20 bg-blue-50">
    <h3 className="text-2xl font-bold text-blue-700 mb-6 text-center">خدماتنا الطبية</h3>
    <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
      {[
        "زراعة وتجميل الأسنان",
        "الباطنة",
        "الجراحة العامة",
        "النساء والتوليد",
        "الأطفال",
        "الجلدية",
        "معمل التحاليل"
      ].map((service, idx) => (
        <div key={idx} className="p-6 bg-white shadow rounded-2xl text-center">
          <h4 className="font-semibold text-lg">{service}</h4>
        </div>
      ))}
    </div>
  </section>

  {/* Blog Section */}
  <section id="blog" className="py-16 px-6 md:px-20 bg-white">
    <h3 className="text-2xl font-bold text-blue-700 mb-6 text-center">مقالات ونصائح طبية</h3>
    <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
      {["5 نصائح للحفاظ على صحة أسنانك", "أهمية الفحص المبكر للأطفال", "دور التغذية في صحة الجلد"].map((post, idx) => (
        <div key={idx} className="p-6 bg-blue-50 rounded-2xl shadow">
          <h4 className="font-semibold text-lg mb-2">{post}</h4>
          <p className="text-sm text-gray-600">اقرأ المزيد...</p>
        </div>
      ))}
    </div>
  </section>

  {/* Contact Section */}
  <section id="contact" className="py-16 px-6 md:px-20 bg-blue-600 text-white">
    <h3 className="text-2xl font-bold mb-6 text-center">احجز موعدك الآن عبر واتساب</h3>
    <div className="max-w-md mx-auto bg-white text-gray-800 p-6 rounded-2xl shadow">
      <form action="https://wa.me/201156141513" method="get" target="_blank" className="space-y-4">
        <input type="text" placeholder="الاسم بالكامل" className="w-full p-3 rounded-lg border border-gray-300" required />
        <input type="tel" placeholder="رقم الهاتف" className="w-full p-3 rounded-lg border border-gray-300" required />
        <select className="w-full p-3 rounded-lg border border-gray-300">
          <option>اختر الخدمة</option>
          <option>زراعة وتجميل الأسنان</option>
          <option>الباطنة</option>
          <option>الجراحة العامة</option>
          <option>النساء والتوليد</option>
          <option>الأطفال</option>
          <option>الجلدية</option>
          <option>معمل التحاليل</option>
        </select>
        <input type="date" className="w-full p-3 rounded-lg border border-gray-300" />
        <button type="submit" className="w-full bg-blue-600 text-white py-3 rounded-lg font-semibold">إرسال عبر واتساب</button>
      </form>
    </div>
    <div className="text-center mt-6">
      <p>📍 الإسكندرية – العصافرة – شارع أطلس أمام أسواق الشريف</p>
      <p>📞 01156141513 – 035536596</p>
    </div>
  </section>

  {/* Footer */}
  <footer className="text-center py-6 bg-gray-100 text-sm text-gray-600">
    © {new Date().getFullYear()} عيادات أطلس الدولية – جميع الحقوق محفوظة
  </footer>
</div>

); }

