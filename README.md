# Controle do acesso de veículos em condomínios
<b> Programa K </b>

Time: Adriano Ferreira, Amir Youssef, Artur Matos, Bernardo Aires, Daired Almeida, Daniel Machado, Emanuelle Passos, Marcelo Henrique

### Ideia:
Visando garantir a segurança em condomínios o acesso de veículos é bem restrito, sendo necessário o preenchimento de registros e outros vários processos burocráticos para a autorização da entrada. Assim, a entrega de comida/objetos ou mesmo a entrada de funcionários de aplicativos de corrida pode ficar demorada e complexa.

### Solução proposta:
Associar a detecção da placa do veículo aos dados em uma planilha referente aos veículos autorizados a entrar no condomínio para que o acesso dele seja mais rápido e fácil, utilizando os conhecimentos obtidos em instructions anteriores.

### Nossa jornada

* **INSTRUCTIONs 1 e 2**: Criamos um notebook prático sobre os princípios da detecção de objetos utilizando YOLOv7 para fazer a **identificação de veículos em vídeo e OCR de suas placas**. Neste notebook, ["object_detection"](https://github.com/Emanuelle-p/object_detection/blob/main/object_detection.ipynb) foram trabalhados os conceitos de Detecção de objetos, YOLOv7, Detecção de contornos e OCR.

* **BUILD 1**: No notebook ["controle_de_acesso_de_veículos_em_condomínios_utilizando_detecção_de_placas"](https://github.com/Emanuelle-p/object_detection/blob/main/controle_de_acesso_de_ve%C3%ADculos_em_condom%C3%ADnios_utilizando_detec%C3%A7%C3%A3o_de_placas.ipynb) foi feita a associação da detecção da placa do veículo aos dados em uma planilha referente aos veículos autorizados a entrar no condomínio. Dessa forma, **quando um veículo é identificado na entrada do condomínio, é feito o OCR de sua placa e o seu acesso é autorizado ou negado**.

* **INSTRUCTION 3**: Visando melhorar o acesso dos usuários (moradores e funcionários do condomínio) a tal sistema desenvolvido no BUILD 1 pensamos em desenvolver uma aplicação web que permitisse facilitar o manejo da base de dados. Para tal, nos dedicamos ao conhecimento e elaboração de um Documento de Requisitos, que pode ser obtido no notebook ["documento_de_requisitos_aplicação_web"](https://github.com/Emanuelle-p/object_detection/blob/main/documento_de_requisitos_aplica%C3%A7%C3%A3o_web.md) e de um protótipo da aplicação.
