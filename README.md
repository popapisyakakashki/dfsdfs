# dfsdfs
import Image from "next/image";

interface ProductCardProps {
  title: string;
  description: string;
  price: number;
  image: string;
}

export default function ProductCard({
  title,
  description,
  price,
  image,
}: ProductCardProps) {
  return (
    <div className="bg-white rounded-3xl p-4 shadow-sm">
      <div className="bg-slate-100 rounded-2xl p-4 flex items-center justify-center">
        <Image
          src={image}
          alt={title}
          width={200}
          height={200}
          className="object-contain"
        />
      </div>

      <h3 className="mt-4 text-xl font-bold text-gray-900">{title}</h3>

      <p className="mt-2 text-sm text-gray-500 leading-relaxed">
        {description}
      </p>

      <p className="mt-2 text-sm text-gray-900">{price} ₽</p>

      <button className="mt-4 bg-blue-900 text-white text-sm px-6 py-2 rounded-full">
        В корзину
      </button>
    </div>
  );
}
