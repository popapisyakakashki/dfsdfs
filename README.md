# dfsdfs
export interface Product {
  id: number;
  title: string;
  description: string;
  price: number;
  image: string;
}

export const products: Product[] = [
  {
    id: 1,
    title: "Наушники Sony WH-1000XM5",
    description: "Беспроводные наушники с активным шумоподавлением",
    price: 29990,
    image: "/headphones.png",
  },
  {
    id: 2,
    title: "Смартфон Samsung Galaxy S24",
    description: "Флагман с ярким AMOLED-экраном",
    price: 79990,
    image: "/phone.png",
  },
  {
    id: 3,
    title: "Ноутбук MacBook Air M3",
    description: "Тонкий и лёгкий ноутбук для работы",
    price: 129990,
    image: "/laptop.png",
  },
  {
    id: 4,
    title: "Умные часы Apple Watch",
    description: "Отслеживание активности и здоровья",
    price: 39990,
    image: "/watch.png",
  },
];
