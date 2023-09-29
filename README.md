# Controle do acesso de veículos em condomínios
<b> Programa K </b>

Time: [Adriano Ferreira](https://www.linkedin.com/in/lopes-adriano/), [Amir Youssef](https://www.linkedin.com/in/amir-youssef-dos-santos-1843b7236/), [Artur Matos](https://www.linkedin.com/in/arturmatos/), [Bernardo Aires](https://www.linkedin.com/in/bernardoaires/), [Daired Almeida](https://www.linkedin.com/in/daired-almeida-cruz-a20163231/), [Daniel Machado](https://www.linkedin.com/in/daniel-machado-9357b6244/), [Emanuelle Passos](https://www.linkedin.com/in/emanuelle-passos-martins-0535a3213/), [Marcelo Henrique](https://www.linkedin.com/in/marcelo-henrique-alves-pereira-sobrinho-7bb0711b8/)

### Ideia:
Visando garantir a segurança em condomínios o acesso de veículos é bem restrito, sendo necessário o preenchimento de registros e outros vários processos burocráticos para a autorização da entrada. Assim, a entrega de comida/objetos ou mesmo a entrada de funcionários de aplicativos de corrida pode ficar demorada e complexa.

### Solução proposta:
Associar a detecção da placa do veículo aos dados em uma planilha referente aos veículos autorizados a entrar no condomínio para que o acesso dele seja mais rápido e fácil.

### Nossa jornada

* **INSTRUCTIONs 1 e 2**: Criamos um notebook prático sobre os princípios da detecção de objetos utilizando YOLOv7 para fazer a `identificação de veículos em vídeo e OCR de suas placas`. Neste notebook, ["object_detection"](https://github.com/Emanuelle-p/object_detection/blob/main/object_detection.ipynb), foram trabalhados os conceitos de **Detecção de objetos**, **YOLOv7**, **Detecção de contornos** e **OCR**.

* **BUILD 1**: No notebook ["controle_de_acesso_de_veículos_em_condomínios_utilizando_detecção_de_placas"](https://github.com/Emanuelle-p/object_detection/blob/main/controle_de_acesso_de_ve%C3%ADculos_em_condom%C3%ADnios_utilizando_detec%C3%A7%C3%A3o_de_placas.ipynb) foi feita a associação da detecção da placa do veículo aos dados em uma planilha referente aos veículos autorizados a entrar no condomínio. Dessa forma, `quando um veículo é identificado na entrada do condomínio, é feito o OCR de sua placa e o seu acesso é autorizado ou negado`.

* **INSTRUCTION 3**: Visando melhorar o acesso dos usuários (moradores e funcionários do condomínio) a tal sistema desenvolvido no BUILD 1 pensamos em desenvolver um `aplicativo` que permitisse facilitar o manejo da base de dados. Para tal, nos dedicamos ao conhecimento e elaboração de um **Documento de Requisitos**, que pode ser obtido no notebook ["documento_de_requisitos"](https://github.com/Emanuelle-p/object_detection/blob/main/documento_de_requisitos_aplica%C3%A7%C3%A3o_web.md) e de um **protótipo** da aplicação, que pode ser acessado em ["protótipo_aplicativo"](https://github.com/Emanuelle-p/object_detection/blob/main/prot%C3%B3tipo_aplica%C3%A7%C3%A3o_web.md). Além disso, criamos materiais de apoio sobre tais etapas com os conhecimentos obtidos: [sobre o documento de requisitos](https://github.com/Emanuelle-p/object_detection/blob/main/material_de_apoio_documento_de_requisitos.md) e [prototipagem usando a ferramenta Figma](https://github.com/Emanuelle-p/object_detection/blob/main/material_de_apoio_prototipagem_figma.md).

* **INSTRUCTION 4**: No repositório [condomínio](https://github.com/lopes-adriano/condominio) foram colocados os projetos elaborados utilizando a ferramenta `Flutter` com o objetivo de ter os primeiros contatos com a criação de um aplicativo **android**. Foram 3 projetos, melhor detalhados no material de apoio [aplicativo](https://github.com/Emanuelle-p/object_detection/blob/main/material_de_apoio_aplicativo.md).

* **BUILD 2**: A detecção de placas contém um fator determinante para que ela seja bem feita ou inviabilizada, isto é, a localização da placa na imagem. Assim, com o objetivo me melhorar a perfomance do modelo foi feita a migração do uso de filtros para o **YOLOv8**, além de um **refinamento dos dados**, eliminando imagens duplicadas (que não necessariamente fossem resultado de um data augmentation) e generalizando ainda mais o dataset incluindo algumas imagem em cenários noturno e chuvoso. Desse modo, obteve-se bons resultados tanto para mAP50 quanto para mAP50-95. Para mais detalhes, [clique aqui para ver o código](https://github.com/Emanuelle-p/object_detection/blob/main/deteccao_placas_yolov8.ipynb).
