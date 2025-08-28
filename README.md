[src_data_products.json](https://github.com/user-attachments/files/22027637/src_data_products.json)
[
  {
    "id": "pack1",
    "title": "Trap Beats Pack Vol. 1",
    "image": "/assets/trap-pack1.png",
    "price": "R$29,90",
    "audio": "/assets/preview-trap1.mp3",
    "description": "Pack completo com beats trap, loops, samples e FLPs editáveis.",
    "buyLink": "https://pag.ae/7Zb6w8XwT"  // Exemplo PagSeguro, pode ser PayPal, Stripe ou Pix
  },
  {
    "id": "pack2",
    "title": "Lo-Fi Essentials",
    "image": "/assets/lofi-pack.png",
    "price": "R$19,90",
    "audio": "/assets/preview-lofi.mp3",
    "description": "Samples Lo-Fi, drum kits exclusivos e projetos base.",
    "buyLink": "https://pag.ae/7Zb6w8XwT"
  }
]
[src_index.css](https://github.com/user-attachments/files/22027646/src_index.css):root {
  --bg: #11131a;
  --primary: #1a1e2e;
  --neon: #40e0d0;
  --text: #f2f2f2;
  --accent: #ff00cc;
}
body {
  background: var(--bg);
  color: var(--text);
  font-family: 'Inter', sans-serif;
  margin: 0;
}
a {
  color: var(--neon);
  text-decoration: none;
}
nav {
  background: var(--primary);
  box-shadow: 0 4px 30px rgba(64,224,208, .07);
}
.menu {
  display: flex;
  gap: 2rem;
  align-items: center;
  justify-content: center;
  padding: 1rem 0;
}
.menu a {
  font-weight: bold;
  letter-spacing: 1px;
  transition: color .2s;
}
.menu a:hover {
  color: var(--accent);
}
.card {
  background: #1a1e2e;
  border-radius: 1rem;
  box-shadow: 0 2px 16px rgba(64,224,208,.08);
  padding: 1.2rem;
  margin: 1rem;
  transition: transform .15s;
}
.card:hover {
  transform: translateY(-4px) scale(1.02);
  box-shadow: 0 4px 24px var(--neon);
}
.neon {
  color: var(--neon);
  text-shadow: 0 0 10px var(--neon), 0 0 2px var(--accent);
}
.btn {
  background: var(--accent);
  color: #fff;
  border: none;
  border-radius: .5rem;
  padding: .7rem 1.5rem;
  font-size: 1rem;
  font-weight: bold;
  cursor: pointer;
  box-shadow: 0 0 8px var(--accent);
  margin-top: 1rem;
  transition: background .15s;
}
.btn:hover {
  background: var(--neon);
  color: #11131a;
}
input, textarea {
  background: #23263b;
  border: 1px solid var(--neon);
  color: var(--text);
  border-radius: .4rem;
  padding: .8rem;
  margin-bottom: .8rem;
  width: 100%;
  font-size: 1rem;
}
@media (max-width: 700px) {import { Link } from "react-router-dom";

export default function Navbar() {
  return (
    <nav>
      <div className="menu">
        <Link to="/"><span className="neon">DJ KABAL</span></Link>
        <Link to="/produtos">Produtos</Link>
        <Link to="/sobre">Sobre</Link>
        <Link to="/contato">Contato</Link>
      </div>export default function Footer() {
  return (
    <footer style={{
      background: "#1a1e2e",
      textAlign: "center",
      padding: "2rem 0",
      marginTop: "3rem",
      fontSize: "1.1rem"
    }}>
      <div>
        <a href="https://instagram.com/sua_rede" target="_blank" rel="noopener noreferrer">Instagram</a> |{" "}
        <a href="https://youtube.com/sua_rede" target="_blank" rel="noopener noreferrer">YouTube</a> |{" "}
        <a href="mailto:seuemail@email.com">Email</a>
      </div>
      <div style={{ marginTop: "1rem", color: "#40e0d0" }}>
        © {new Date().getFullYear()} DJ KABAL. Todos os direitos reservados.
      </div>
    </footer>
  );
}
    </nav>
  );
}
  .menu { flex-direction: column; gap: 1rem; }
  .cards { grid-template-columns: 1fr !important; }
}
