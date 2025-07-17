import { useEffect, useState } from 'react';
import Navbar from '../../components/Navbar';

export default function BscCsSem1() {
  const [unlocked, setUnlocked] = useState(false);

  useEffect(() => {
    const isPaid = localStorage.getItem('sem1_paid');
    if (isPaid === 'true') setUnlocked(true);
  }, []);

  const handlePayment = async () => {
    const res = await fetch('/api/create-order', { method: 'POST' });
    const order = await res.json();

    const options = {
      key: 'YOUR_KEY_ID', // From Razorpay Dashboard
      amount: order.amount,
      currency: order.currency,
      name: 'TextbookVideo Hub',
      description: 'Unlock BSc CS Sem 1',
      order_id: order.id,
      handler: function (response) {
        // ✅ Store unlock info
        localStorage.setItem('sem1_paid', 'true');
        setUnlocked(true);
        alert('Payment Successful');
      },
      prefill: {
        email: "testuser@example.com"
      },
      theme: {
        color: "#3399cc"
      }
    };

    const rzp = new window.Razorpay(options);
    rzp.open();
  };

  useEffect(() => {
    if (!window.Razorpay) {
      const script = document.createElement('script');
      script.src = "https://checkout.razorpay.com/v1/checkout.js";
      script.async = true;
      document.body.appendChild(script);
    }
  }, []);

  const subjects = [
    { name: "Mathematics I", file: "/pdfs/math1.pdf" },
    { name: "Physics", file: "/pdfs/physics.pdf" },
    // Add rest...
  ];

  return (
    <>
      <Navbar />
      <div className="p-8">
        <h1 className="text-2xl font-semibold mb-6">BSc CS - Semester 1</h1>

        {!unlocked ? (
          <div className="text-center">
            <p className="mb-4">Unlock this semester for ₹30</p>
            <button onClick={handlePayment} className="bg-blue-600 text-white px-6 py-2">Pay & Unlock</button>
          </div>
        ) : (
          <ul className="space-y-3">
            {subjects.map((subj, i) => (
              <li key={i} className="border-b pb-2">
                <span className="font-medium">{subj.name}:</span>
                <a href={subj.file} className="text-blue-600 hover:underline ml-2" target="_blank" rel="noreferrer">View PDF</a>
              </li>
            ))}
          </ul>
        )}
      </div>
    </>
  );
}
