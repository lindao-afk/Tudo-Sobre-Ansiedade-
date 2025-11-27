<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Caminho da Serenidade - Domine Sua Ansiedade</title>
    <style>
        /* Reset e configurações gerais */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f8f9fa;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Cores da paleta */
        :root {
            --primary: #5d8aa8; /* Azul suave */
            --secondary: #6b8e6b; /* Verde suave */
            --accent: #9f86c0; /* Lilás suave */
            --light: #f0f4f8;
            --dark: #2c3e50;
            --text: #333333;
        }
        
        /* Botões */
        .btn {
            display: inline-block;
            padding: 15px 30px;
            background: linear-gradient(135deg, var(--primary), var(--accent));
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            font-size: 18px;
            text-align: center;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(93, 138, 168, 0.3);
            border: none;
            cursor: pointer;
        }
        
        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(93, 138, 168, 0.4);
        }
        
        .btn-secondary {
            background: linear-gradient(135deg, var(--secondary), #7aa97a);
        }
        
        /* Seções */
        section {
            padding: 80px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
            color: var(--dark);
            font-size: 36px;
            position: relative;
        }
        
        .section-title:after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background: linear-gradient(to right, var(--primary), var(--accent));
            margin: 15px auto;
            border-radius: 2px;
        }
        
        /* Header */
        header {
            background: linear-gradient(135deg, var(--primary), var(--accent));
            color: white;
            padding: 100px 0;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        header:before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxMDAlIiBoZWlnaHQ9IjEwMCUiPjxkZWZzPjxwYXR0ZXJuIGlkPSJwYXR0ZXJuIiB3aWR0aD0iNDAiIGhlaWdodD0iNDAiIHBhdHRlcm5Vbml0cz0idXNlclNwYWNlT25Vc2UiIHBhdHRlcm5UcmFuc2Zvcm09InJvdGF0ZSg0NSkiPjxyZWN0IHg9IjAiIHk9IjAiIHdpZHRoPSIyMCIgaGVpZ2h0PSIyMCIgZmlsbD0icmdiYSgyNTUsMjU1LDI1NSwwLjA1KSIvPjwvcGF0dGVybj48L2RlZnM+PHJlY3QgZmlsbD0idXJsKCNwYXR0ZXJuKSIgd2lkdGg9IjEwMCUiIGhlaWdodD0iMTAwJSIvPjwvc3ZnPg==');
        }
        
        .header-content {
            position: relative;
            z-index: 1;
            max-width: 800px;
            margin: 0 auto;
        }
        
        h1 {
            font-size: 48px;
            margin-bottom: 20px;
            text-shadow: 1px 1px 3px rgba(0,0,0,0.2);
        }
        
        .subheadline {
            font-size: 24px;
            margin-bottom: 30px;
            font-weight: 300;
        }
        
        .price-tag {
            background-color: rgba(255,255,255,0.2);
            display: inline-block;
            padding: 10px 25px;
            border-radius: 30px;
            margin: 20px 0;
            font-size: 22px;
            backdrop-filter: blur(5px);
        }
        
        /* Benefícios */
        .benefits {
            background-color: white;
        }
        
        .benefits-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .benefit-card {
            background-color: var(--light);
            padding: 30px;
            border-radius: 10px;
            text-align: center;
            transition: transform 0.3s ease;
        }
        
        .benefit-card:hover {
            transform: translateY(-10px);
        }
        
        .benefit-icon {
            font-size: 40px;
            color: var(--primary);
            margin-bottom: 20px;
        }
        
        .benefit-card h3 {
            margin-bottom: 15px;
            color: var(--dark);
        }
        
        /* Conteúdo do ebook */
        .ebook-content {
            background-color: var(--light);
        }
        
        .modules {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .module {
            background-color: white;
            border-radius: 10px;
            padding: 25px;
            margin-bottom: 20px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            border-left: 5px solid var(--accent);
        }
        
        .module h3 {
            color: var(--dark);
            margin-bottom: 10px;
        }
        
        /* Depoimentos */
        .testimonials {
            background-color: white;
        }
        
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .testimonial-card {
            background-color: var(--light);
            padding: 30px;
            border-radius: 10px;
            position: relative;
        }
        
        .testimonial-card:before {
            content: '"';
            font-size: 60px;
            color: var(--primary);
            opacity: 0.2;
            position: absolute;
            top: 10px;
            left: 20px;
        }
        
        .testimonial-text {
            font-style: italic;
            margin-bottom: 20px;
        }
        
        .testimonial-author {
            font-weight: bold;
            color: var(--dark);
        }
        
        /* Garantia */
        .guarantee {
            background: linear-gradient(135deg, var(--secondary), #7aa97a);
            color: white;
            text-align: center;
        }
        
        .guarantee-box {
            background-color: rgba(255,255,255,0.1);
            padding: 40px;
            border-radius: 15px;
            max-width: 800px;
            margin: 0 auto;
            backdrop-filter: blur(5px);
        }
        
        .guarantee-icon {
            font-size: 60px;
            margin-bottom: 20px;
        }
        
        /* CTA final */
        .final-cta {
            background-color: var(--dark);
            color: white;
            text-align: center;
        }
        
        .urgency {
            background-color: #e74c3c;
            color: white;
            padding: 10px 20px;
            border-radius: 5px;
            display: inline-block;
            margin-bottom: 20px;
            font-weight: bold;
        }
        
        /* Footer */
        footer {
            background-color: #1a252f;
            color: #95a5a6;
            padding: 40px 0;
            text-align: center;
        }
        
        /* Responsividade */
        @media (max-width: 768px) {
            h1 {
                font-size: 36px;
            }
            
            .subheadline {
                font-size: 20px;
            }
            
            section {
                padding: 60px 0;
            }
            
            .section-title {
                font-size: 28px;
            }
        }
    </style>
</head>
<body>
    <!-- Header com CTA principal -->
    <header>
        <div class="container">
            <div class="header-content">
                <h1>Domine Sua Ansiedade e Reconquiste a Paz Interior</h1>
                <p class="subheadline">Descubra o método passo a passo para controlar a ansiedade e viver uma vida mais leve e plena</p>
                <div class="price-tag">Apenas R$ 19,90</div>
                <a href="#cta-final" class="btn">Quero Controlar Minha Ansiedade Agora</a>
                <p style="margin-top: 20px; font-size: 14px;">Garantia de 7 dias ou seu dinheiro de volta</p>
            </div>
        </div>
    </header>

    <!-- Seção de problema/solução -->
    <section>
        <div class="container">
            <h2 class="section-title">Você Também Sente Isso?</h2>
            <div style="max-width: 800px; margin: 0 auto;">
                <p style="font-size: 18px; margin-bottom: 20px;">Acorda com o coração acelerado, mesmo sem motivo aparente? Sua mente não para de criar cenários catastróficos? Sente um aperto no peito que parece não ter fim?</p>
                <p style="font-size: 18px; margin-bottom: 20px;">A ansiedade rouba sua paz, sua energia e sua capacidade de aproveitar os momentos simples da vida. Mas você não precisa continuar vivendo assim.</p>
                <p style="font-size: 18px; margin-bottom: 30px;">Eu já estive onde você está agora. Passei anos lutando contra a ansiedade, até descobrir um caminho que transformou completamente minha relação com meus pensamentos e emoções.</p>
                <div style="text-align: center;">
                    <a href="#cta-final" class="btn">Quero Conhecer Esse Caminho</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Seção de benefícios -->
    <section class="benefits">
        <div class="container">
            <h2 class="section-title">O Que Você Vai Alcançar</h2>
            <div class="benefits-grid">
                <div class="benefit-card">
                    <div class="benefit-icon">😌</div>
                    <h3>Paz Mental</h3>
                    <p>Aprenda técnicas para acalmar sua mente e reduzir o fluxo incessante de pensamentos ansiosos.</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">💪</div>
                    <h3>Controle Emocional</h3>
                    <p>Desenvolva habilidades para gerenciar suas emoções e não ser mais dominado por elas.</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">🌅</div>
                    <h3>Qualidade de Vida</h3>
                    <p>Recupere o prazer nas atividades cotidianas e volte a aproveitar a vida plenamente.</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">🛌</div>
                    <h3>Sono Restaurador</h3>
                    <p>Durma melhor e acorde revigorado, sem aquela sensação de cansaço constante.</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">🤝</div>
                    <h3>Relacionamentos Melhores</h3>
                    <p>Esteja presente de verdade nas suas relações, sem a interferência da ansiedade.</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">🎯</div>
                    <h3>Foco e Produtividade</h3>
                    <p>Recupere sua capacidade de concentração e realize mais em menos tempo.</p>
                </div>
            </div>
            <div style="text-align: center; margin-top: 40px;">
                <a href="#cta-final" class="btn">Quero Esses Benefícios</a>
            </div>
        </div>
    </section>

    <!-- Seção sobre o ebook -->
    <section class="ebook-content">
        <div class="container">
            <h2 class="section-title">O Que Você Vai Encontrar no Ebook</h2>
            <div class="modules">
                <div class="module">
                    <h3>Módulo 1: Entendendo a Ansiedade</h3>
                    <p>Compreenda os mecanismos da ansiedade, identificando seus gatilhos e padrões de pensamento.</p>
                </div>
                <div class="module">
                    <h3>Módulo 2: Técnicas de Respiração e Grounding</h3>
                    <p>Métodos práticos para acalmar o sistema nervoso em momentos de crise ansiosa.</p>
                </div>
                <div class="module">
                    <h3>Módulo 3: Reestruturação Cognitiva</h3>
                    <p>Aprenda a identificar e desafiar pensamentos distorcidos que alimentam a ansiedade.</p>
                </div>
                <div class="module">
                    <h3>Módulo 4: Mindfulness e Aceitação</h3>
                    <p>Pratique a atenção plena para viver o presente sem julgamentos.</p>
                </div>
                <div class="module">
                    <h3>Módulo 5: Hábitos para uma Mente Saudável</h3>
                    <p>Desenvolva um estilo de vida que previne a ansiedade e promove bem-estar mental.</p>
                </div>
                <div class="module">
                    <h3>Bônus: Guia de Emergência para Crises de Ansiedade</h3>
                    <p>Um protocolo passo a passo para quando a ansiedade parecer avassaladora.</p>
                </div>
            </div>
            <div style="text-align: center; margin-top: 40px;">
                <a href="#cta-final" class="btn">Quero Acessar Todo Este Conteúdo</a>
            </div>
        </div>
    </section>

    <!-- Seção de depoimentos -->
    <section class="testimonials">
        <div class="container">
            <h2 class="section-title">O Que Nossos Leitores Dizem</h2>
            <div class="testimonial-grid">
                <div class="testimonial-card">
                    <p class="testimonial-text">"Depois de anos lutando contra a ansiedade, finalmente encontrei algo que realmente funciona. As técnicas são simples mas poderosas. Minha qualidade de vida melhorou 100%."</p>
                    <p class="testimonial-author">Marina S., 32 anos</p>
                </div>
                <div class="testimonial-card">
                    <p class="testimonial-text">"Comprei com ceticismo, mas me surpreendi. Em menos de 2 semanas já sentia diferença. Aprendi a não lutar contra a ansiedade, mas a entendê-la e acalmá-la."</p>
                    <p class="testimonial-author">Ricardo L., 41 anos</p>
                </div>
                <div class="testimonial-card">
                    <p class="testimonial-text">"O módulo sobre respiração salvou minha vida durante uma crise de pânico. Agora tenho ferramentas para lidar com a ansiedade em qualquer situação."</p>
                    <p class="testimonial-author">Camila R., 28 anos</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Seção de garantia -->
    <section class="guarantee">
        <div class="container">
            <div class="guarantee-box">
                <div class="guarantee-icon">🔒</div>
                <h2 style="margin-bottom: 20px;">Garantia Incondicional de 7 Dias</h2>
                <p style="font-size: 18px; margin-bottom: 20px;">Estou tão confiante de que este ebook vai transformar sua relação com a ansiedade que ofereço uma garantia total. Se em 7 dias você não sentir uma melhora significativa, devolvo 100% do seu investimento.</p>
                <p style="font-size: 18px;">Sem perguntas, sem burocracia. É arriscar nada para ganhar tudo.</p>
            </div>
        </div>
    </section>

    <!-- CTA final -->
    <section class="final-cta" id="cta-final">
        <div class="container">
            <div class="urgency">OFERTA ESPECIAL POR TEMPO LIMITADO</div>
            <h2 style="margin-bottom: 20px;">Invista em Sua Paz Interior por Apenas R$ 19,90</h2>
            <p style="font-size: 18px; margin-bottom: 30px; max-width: 800px; margin-left: auto; margin-right: auto;">Menos do que você gasta em uma refeição fora, mas com potencial para transformar completamente sua qualidade de vida.</p>
            <a href="#" class="btn btn-secondary">Quero Começar Minha Transformação</a>
            <p style="margin-top: 20px; font-size: 14px;">✓ Acesso imediato após a compra ✓ Download em PDF e EPUB ✓ Bônus exclusivos incluídos</p>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>© 2023 Caminho da Serenidade. Todos os direitos reservados.</p>
            <p style="margin-top: 10px; font-size: 14px;">Este produto não substitui acompanhamento médico ou psicológico profissional.</p>
        </div>
    </footer>
</body>
</html>
