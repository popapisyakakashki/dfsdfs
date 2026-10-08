# dfsdfs
import ProductCard from "./components/ProductCard";
import { products } from "./data/products";

export default function Home() {
  return (
    <main className="max-w-7xl mx-auto px-4 py-8">
      <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-5">
        {products.map((product) => (
          <ProductCard
            key={product.id}
            title={product.title}
            description={product.description}
            price={product.price}
            image={product.image}
          />
        ))}
      </div>

      <div className="flex justify-center mt-10">
        <button className="bg-blue-900 text-white uppercase rounded-full px-16 py-3 transition-colors hover:bg-blue-800">
          Смотреть всю коллекцию
        </button>
      </div>
    </main>
  );
}
