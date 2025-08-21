
import React from "react";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { Phone, Mail, Instagram, ArrowRight, Palette, Monitor, Hotel, Star, Award, Users } from "lucide-react";

export default function Home() {
  return (
    <div className="min-h-screen">
      {/* Hero Section */}
      <section className="relative min-h-screen flex items-center justify-center bg-gradient-to-br from-green-50 via-white to-orange-50 leaf-pattern">
        <div className="absolute inset-0 bg-gradient-to-r from-green-800/5 to-orange-500/5"></div>
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative">
          <div className="text-center max-w-4xl mx-auto">
            {/* Logo Grande */}
            <div className="mb-8 flex justify-center">
              <img
                src="https://qtrypzzcjebvfcihiynt.supabase.co/storage/v1/object/public/base44-prod/public/29d6809bc_Identidade-Visual---GG_0000_LOGO.png"
                alt="Gandarela Logo"
                className="w-32 h-32 rounded-2xl shadow-2xl"
              />
            </div>

            <h1 className="text-5xl lg:text-7xl font-bold mb-6 tracking-tight text-green-800">
              GANDARELA
            </h1>
            <p className="text-xl lg:text-2xl text-gray-600 mb-8 uppercase tracking-wider font-medium">
              Comunicação Visual
            </p>
            <p className="text-lg lg:text-xl text-gray-700 mb-12 leading-relaxed max-w-3xl mx-auto">
              Transformamos suas ideias em comunicação visual impactante. 
              Especializados em materiais gráficos, design digital e soluções exclusivas para hotelaria.
            </p>

            <div className="flex flex-col sm:flex-row gap-4 justify-center">
              <Button size="lg" className="bg-green-800 hover:bg-green-900 text-white px-8 py-4 text-lg">
                <Phone className="w-5 h-5 mr-2" />
                Solicitar Orçamento
              </Button>
              <Button size="lg" variant="outline" className="border-orange-500 text-orange-500 hover:bg-orange-50 px-8 py-4 text-lg">
                Ver Portfólio
                <ArrowRight className="w-5 h-5 ml-2" />
              </Button>
            </div>
          </div>
        </div>
      </section>

      {/* Services Section */}
      <section id="servicos" className="py-24 bg-white">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="text-center mb-16">
            <h2 className="text-4xl lg:text-5xl font-bold text-gray-900 mb-6">
              Nossos Serviços
            </h2>
            <p className="text-xl text-gray-600 max-w-3xl mx-auto leading-relaxed">
              Oferecemos soluções completas em comunicação visual, desde design gráfico tradicional 
              até materiais especializados para hotelaria.
            </p>
          </div>

          <div className="grid lg:grid-cols-3 gap-8">
            <Card className="group hover:shadow-2xl transition-all duration-300 border-0 shadow-lg bg-gradient-to-br from-white to-gray-50">
              <CardContent className="p-8">
                <div className="w-16 h-16 rounded-2xl bg-green-100 flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
                  <Palette className="w-8 h-8 text-green-800" />
                </div>
                <h3 className="text-2xl font-bold text-gray-900 mb-4">Design Gráfico</h3>
                <p className="text-gray-600 mb-6 leading-relaxed">
                  Criação de identidade visual, logotipos, cartões de visita, flyers, banners e 
                  todo tipo de material gráfico para sua empresa.
                </p>
                <ul className="text-sm text-gray-600 space-y-2">
                  <li>• Identidade Visual</li>
                  <li>• Material Impresso</li>
                  <li>• Logotipos e Marcas</li>
                  <li>• Cartões e Flyers</li>
                </ul>
              </CardContent>
            </Card>

            <Card className="group hover:shadow-2xl transition-all duration-300 border-0 shadow-lg bg-gradient-to-br from-white to-orange-50">
              <CardContent className="p-8">
                <div className="w-16 h-16 rounded-2xl bg-orange-100 flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
                  <Monitor className="w-8 h-8 text-orange-600" />
                </div>
                <h3 className="text-2xl font-bold text-gray-900 mb-4">Design Digital</h3>
                <p className="text-gray-600 mb-6 leading-relaxed">
                  Criação de conteúdo digital para redes sociais, sites, e-commerce e 
                  todas as plataformas digitais da sua empresa.
                </p>
                <ul className="text-sm text-gray-600 space-y-2">
                  <li>• Posts para Redes Sociais</li>
                  <li>• Banners Digitais</li>
                  <li>• Design para E-commerce</li>
                  <li>• Materiais Online</li>
                </ul>
              </CardContent>
            </Card>

            <Card className="group hover:shadow-2xl transition-all duration-300 border-0 shadow-lg bg-gradient-to-br from-white to-green-50">
              <CardContent className="p-8">
                <div className="w-16 h-16 rounded-2xl bg-green-100 flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
                  <Hotel className="w-8 h-8 text-green-800" />
                </div>
                <h3 className="text-2xl font-bold text-gray-900 mb-4">Materiais para Hotelaria</h3>
                <p className="text-gray-600 mb-6 leading-relaxed">
                  Soluções especializadas para hotéis, pousadas e estabelecimentos do setor, 
                  criando experiências visuais únicas para seus hóspedes.
                </p>
                <ul className="text-sm text-gray-600 space-y-2">
                  <li>• Cardápios e Menus</li>
                  <li>• Sinalização Interna</li>
                  <li>• Amenities Personalizados</li>
                  <li>• Material de Recepção</li>
                </ul>
              </CardContent>
            </Card>
          </div>
        </div>
      </section>

      {/* Portfolio Section */}
      <section id="portfolio" className="py-24 bg-gradient-to-b from-gray-50 to-white">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="text-center mb-16">
            <h2 className="text-4xl lg:text-5xl font-bold text-gray-900 mb-6">
              Portfólio
            </h2>
            <p className="text-xl text-gray-600 max-w-3xl mx-auto">
              Alguns dos nossos trabalhos mais recentes e projetos que demonstram 
              nossa expertise em comunicação visual.
            </p>
          </div>

          <div className="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
            {[
              { title: "Identidade Visual Completa", category: "Branding", image: "https://images.unsplash.com/photo-1558655146-d09347e92766?w=400&h=300&fit=crop" },
              { title: "Material para Hotelaria", category: "Hotelaria", image: "https://images.unsplash.com/photo-1564013799919-ab600027ffc6?w=400&h=300&fit=crop" },
              { title: "Design Digital", category: "Digital", image: "https://images.unsplash.com/photo-1561070791-2526d30994b5?w=400&h=300&fit=crop" },
              { title: "Materiais Impressos", category: "Impresso", image: "https://images.unsplash.com/photo-1586953208448-b95a79798f07?w=400&h=300&fit=crop" },
              { title: "Sinalização", category: "Sinalização", image: "https://images.unsplash.com/photo-1497366216548-37526070297c?w=400&h=300&fit=crop" },
              { title: "Cardápios", category: "Hotelaria", image: "https://images.unsplash.com/photo-1414235077428-338989a2e8c0?w=400&h=300&fit=crop" }
            ].map((project, index) => (
              <Card key={index} className="group hover:shadow-2xl transition-all duration-300 overflow-hidden border-0 shadow-lg">
                <div className="aspect-[4/3] overflow-hidden">
                  <img 
                    src={project.image} 
                    alt={project.title}
                    className="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500"
                  />
                </div>
                <CardContent className="p-6">
                  <span className="inline-block px-3 py-1 bg-orange-100 text-orange-800 text-sm font-medium rounded-full mb-3">
                    {project.category}
                  </span>
                  <h3 className="text-xl font-bold text-gray-900">{project.title}</h3>
                </CardContent>
              </Card>
            ))}
          </div>
        </div>
      </section>

      {/* About Section */}
      <section id="sobre" className="py-24 bg-white">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="grid lg:grid-cols-2 gap-16 items-center">
            <div>
              <h2 className="text-4xl lg:text-5xl font-bold text-gray-900 mb-8">
                Felipe Gandarela
              </h2>
              <p className="text-xl text-gray-600 mb-6 leading-relaxed">
                Designer gráfico especializado em comunicação visual com foco em resultados. 
                Com anos de experiência no mercado, desenvolvo soluções criativas e funcionais 
                para empresas de todos os segmentos.
              </p>
              <p className="text-lg text-gray-600 mb-8 leading-relaxed">
                Minha especialidade em materiais para hotelaria me permite criar experiências 
                visuais únicas que elevam a percepção de marca dos estabelecimentos.
              </p>
              
              <div className="grid sm:grid-cols-3 gap-6 mb-8">
                <div className="text-center">
                  <Award className="w-8 h-8 text-orange-500 mx-auto mb-2" />
                  <div className="text-2xl font-bold text-gray-900">50+</div>
                  <div className="text-sm text-gray-600">Projetos Entregues</div>
                </div>
                <div className="text-center">
                  <Users className="w-8 h-8 text-green-800 mx-auto mb-2" />
                  <div className="text-2xl font-bold text-gray-900">30+</div>
                  <div className="text-sm text-gray-600">Clientes Satisfeitos</div>
                </div>
                <div className="text-center">
                  <Star className="w-8 h-8 text-orange-500 mx-auto mb-2" />
                  <div className="text-2xl font-bold text-gray-900">5★</div>
                  <div className="text-sm text-gray-600">Avaliação Média</div>
                </div>
              </div>
            </div>

            <div className="relative">
              <div className="aspect-square rounded-3xl bg-gradient-to-br from-green-800 to-green-900 p-8 shadow-2xl">
                <div className="w-full h-full rounded-2xl bg-gradient-to-br from-orange-400 to-orange-500 flex items-center justify-center">
                  <div className="text-white text-6xl font-bold">FG</div>
                </div>
              </div>
              <div className="absolute -bottom-6 -right-6 w-32 h-32 bg-orange-500 rounded-full opacity-20"></div>
              <div className="absolute -top-6 -left-6 w-24 h-24 bg-green-800 rounded-full opacity-20"></div>
            </div>
          </div>
        </div>
      </section>

      {/* Contact Section */}
      <section id="contato" className="py-24 bg-gradient-to-br from-green-800 to-green-900 text-white">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="text-center mb-16">
            <h2 className="text-4xl lg:text-5xl font-bold mb-6">
              Vamos Conversar?
            </h2>
            <p className="text-xl opacity-90 max-w-3xl mx-auto">
              Pronto para transformar sua comunicação visual? Entre em contato e vamos 
              desenvolver algo incrível juntos.
            </p>
          </div>

          <div className="grid lg:grid-cols-3 gap-8">
            <Card className="bg-white bg-opacity-10 backdrop-blur border-white border-opacity-20 hover:bg-opacity-20 transition-all duration-300">
              <CardContent className="p-8 text-center">
                <div className="w-16 h-16 rounded-2xl bg-orange-500 flex items-center justify-center mx-auto mb-6">
                  <Phone className="w-8 h-8 text-white" />
                </div>
                <h3 className="text-xl font-bold mb-4">Telefone</h3>
                <p className="text-lg opacity-90">(31) 9 9104-5771</p>
                <Button variant="outline" className="mt-4 border-white text-white hover:bg-white hover:text-green-800">
                  Ligar Agora
                </Button>
              </CardContent>
            </Card>

            <Card className="bg-white bg-opacity-10 backdrop-blur border-white border-opacity-20 hover:bg-opacity-20 transition-all duration-300">
              <CardContent className="p-8 text-center">
                <div className="w-16 h-16 rounded-2xl bg-orange-500 flex items-center justify-center mx-auto mb-6">
                  <Mail className="w-8 h-8 text-white" />
                </div>
                <h3 className="text-xl font-bold mb-4">E-mail</h3>
                <p className="text-lg opacity-90 break-all">flsrioacima@gmail.com</p>
                <Button variant="outline" className="mt-4 border-white text-white hover:bg-white hover:text-green-800">
                  Enviar E-mail
                </Button>
              </CardContent>
            </Card>

            <Card className="bg-white bg-opacity-10 backdrop-blur border-white border-opacity-20 hover:bg-opacity-20 transition-all duration-300">
              <CardContent className="p-8 text-center">
                <div className="w-16 h-16 rounded-2xl bg-orange-500 flex items-center justify-center mx-auto mb-6">
                  <Instagram className="w-8 h-8 text-white" />
                </div>
                <h3 className="text-xl font-bold mb-4">Instagram</h3>
                <p className="text-lg opacity-90">@graficagandarela</p>
                <Button variant="outline" className="mt-4 border-white text-white hover:bg-white hover:text-green-800">
                  Seguir
                </Button>
              </CardContent>
            </Card>
          </div>
        </div>
      </section>
    </div>
  );
}
