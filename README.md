export default function MercadoLivreAffiliateSite(https://meli.la/2WyMDxf) {
  const products = [
    {
      title: 'Copo Térmico Stanley',
      description: 'O copo térmico mais vendido para bebidas geladas.',
      image: 'https://images.unsplash.com/photo-1514228742587-6b1558fcf93a?q=80&w=1200&auto=format&fit=crop',
      link: 'https://mercadolivre.com.br/meli.la/2WyMDxf-1',
      price: 'R$ 89,90',
      category: 'Mais Vendidos'
    },
    {
      title: 'Smartphone Android Premium',
      description: 'Celular com ótimo desempenho e câmera profissional.',
      image: 'https://images.unsplash.com/photo-1511707171634-5f897ff02aa9?q=80&w=1200&auto=format&fit=crop',
      link: 'https://mercadolivre.com.br/meli.la/2WyMDxf-2',
      price: 'R$ 1.299,90',
      category: 'Eletrônicos'
    },
    {
      title: 'Aparelho de Barbear Profissional',
      description: 'Barbear rápido e preciso para o dia a dia.',
      image: 'https://images.unsplash.com/photo-1519014816548-bf5fe059798b?q=80&w=1200&auto=format&fit=crop',
      link: 'https://mercadolivre.com.br/meli.la/2WyMDxf-3',
      price: 'R$ 129,90',
      category: 'Cuidados Pessoais'
    },
    {
      title: 'Fone Bluetooth Gamer',
      description: 'Som imersivo e bateria de longa duração.',
      image: 'https://images.unsplash.com/photo-1505740420928-5e560c06d30e?q=80&w=1200&auto=format&fit=crop',
      link: 'https://mercadolivre.com.br/meli.la/2WyMDxf-4',
      price: 'R$ 199,90',
      category: 'Gamer'
    },
    {
      title: 'Notebook Ultrafino',
      description: 'Ideal para trabalho, estudos e produtividade.',
      image: 'https://images.unsplash.com/photo-1496181133206-80ce9b88a853?q=80&w=1200&auto=format&fit=crop',
      link: 'https://mercadolivre.com.br/meli.la/2WyMDxf-5',
      price: 'R$ 2.899,90',
      category: 'Tecnologia'
    },
    {
      title: 'Air Fryer Digital',
      description: 'Prepare receitas rápidas e saudáveis.',
      image: 'https://images.unsplash.com/photo-1585515656973-6e9e7f1b9f8f?q=80&w=1200&auto=format&fit=crop',
      link: 'https://mercadolivre.com.br/meli.la/2WyMDxf-6',
      price: 'R$ 349,90',
      category: 'Casa'
    }
  ];

  return (
    <div className="min-h-screen bg-gray-100 text-gray-900">
      <header className="bg-yellow-400 shadow-lg">
        <div className="max-w-7xl mx-auto px-6 py-8 flex flex-col md:flex-row justify-between items-center">
          <div>
            <h1 className="text-4xl font-bold">Edjo Ofertas</h1>
            <p className="text-lg mt-2">As melhores ofertas do Mercado Livre em um só lugar</p>
          </div>

          <a
            href="https://www.mercadolivre.com.br"
            target="_blank"
            className="mt-4 md:mt-0 bg-black text-white px-6 py-3 rounded-2xl font-semibold hover:scale-105 transition"
          >
            Ver Promoções
          </a>
        </div>
      </header>

      <section className="max-w-7xl mx-auto px-6 py-12">
        <div className="text-center mb-10">
          <h2 className="text-3xl font-bold">Produtos em Destaque</h2>
          <p className="text-gray-600 mt-2">Escolha os produtos mais vendidos para aumentar suas comissões.</p>
        </div>

        <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
          {products.map((product, index) => (
            <div
              key={index}
              className="bg-white rounded-3xl shadow-lg overflow-hidden hover:-translate-y-2 transition"
            >
              <img
                src={product.image}
                alt={product.title}
                className="w-full h-64 object-cover"
              />

              <div className="p-6">
                <h3 className="text-2xl font-bold">{product.title}</h3>
                <p className="text-gray-600 mt-3">{product.description}</p>

                <div className="mt-4 flex items-center justify-between">
                  <span className="text-2xl font-bold text-green-600">{product.price}</span>
                </div>

                <a
                  href={product.link}
                  target="_blank"
                  className="block mt-6 bg-yellow-400 hover:bg-yellow-500 text-center py-3 rounded-2xl font-bold transition"
                >
                  Comprar Agora
                </a>
              </div>
            </div>
          ))}
        </div>
      </section>

      <section className="bg-black text-white py-16 mt-10">
        <div className="max-w-5xl mx-auto px-6 text-center">
          <h2 className="text-4xl font-bold">Ganhe com Produtos Virais</h2>
          <p className="mt-4 text-lg text-gray-300">
            Divulgue produtos do Mercado Livre com seus links de afiliado e aumente suas vendas nas redes sociais.
          </p>

          <div className="mt-8 flex flex-col md:flex-row gap-4 justify-center">
            <button className="bg-yellow-400 text-black px-8 py-4 rounded-2xl font-bold hover:scale-105 transition">
              Produtos Mais Vendidos
            </button>

            <button className="border border-white px-8 py-4 rounded-2xl font-bold hover:bg-white hover:text-black transition">
              Promoções do Dia
            </button>
          </div>
        </div>
      </section>

      <footer className="bg-gray-900 text-gray-300 py-8 text-center">
        <p>© 2026 Edjo ofertas - Site de Afiliados Mercado Livre</p>
      </footer>
    </div>
  );
}
