// ✅ Razorpay Order API (pages/api/create-order.js)
import Razorpay from 'razorpay';

const razorpay = new Razorpay({
  key_id: 'YOUR_KEY_ID',
  key_secret: 'YOUR_SECRET_KEY',
});

export default async function handler(req, res) {
  if (req.method === 'POST') {
    const options = {
      amount: 3000, // ₹30 in paise
      currency: "INR",
      receipt: "sem1_payment",
    };

    try {
      const order = await razorpay.orders.create(options);
      res.status(200).json(order);
    } catch (err) {
      res.status(500).json({ error: "Failed to create order" });
    }
  } else {
    res.status(405).json({ error: "Method not allowed" });
  }
}
