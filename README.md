<h3 align="center">
COGNITIVE AND SEMANTIC COMPUTATION & IOT
</h3>
<p align="center">
NAC 10 - Trabalho sobre Redes Convolutivas
</p>
<p align="center">
  <img alt="Repository size" src="https://img.shields.io/github/repo-size/robertosousa1/skin-cancer-detection.svg">
  </a>
  <a href="https://github.com/robertosousa1/skin-cancer-detection/issues">
    <img alt="Repository issues" src="https://img.shields.io/github/issues/robertosousa1/skin-cancer-detection.svg">
  </a>
</p>

## [](#license):memo: Grupo
- Gustavo Pinilha - RM 78298
- João Fogaça -
- Leonardo Kodama - RM 78034
- Roberto Alves - RM 77831
- Rodrigo Lebrão - 

## [](#how-to-contribute):pencil2: Questões

-   Qual arquitetura foi utilizada e por quê?
	- A arquitetura escolhida foi a **InceptionV3** pelas seguintes características:
		- Compatibilidade com modelos pré-treinado oferecido pelo Keras
		-  Permite adicionar camadas ao final para customizar as saídas da rede
		-  Propaga informações de rótulos na rede (compatibilidade de ação com o *Batch Normalization*)

-   Camadas convolutivas:
	- Usamos o **GlobalAveragePooling2D** para adicionar uma camada global de Pooling
	- Usamos o **Dense** para adicionar uma camada densa na camada final
	- Usamos o **Dropout** para regularização e evitar overfitting 
  
- Teste diferentes funções de ativação.
	- **Softmax**

   <img alt="metrics" src="https://res.cloudinary.com/robertosousa1/image/upload/v1604366328/tcc/download_uaqv76.png" width="520px" />
   <img alt="metrics" src="https://res.cloudinary.com/robertosousa1/image/upload/v1604366328/tcc/download_1_w19a6o.png" width="520px" />
   <img alt="metrics" src="https://res.cloudinary.com/robertosousa1/image/upload/v1604366328/tcc/download_2_kferdo.png" width="520px" />
   <img alt="metrics" src="https://res.cloudinary.com/robertosousa1/image/upload/v1604366328/tcc/Captura_de_Tela_2020-11-02_a%CC%80s_21.54.13_nk2swc.png" width="520px" />

	- **ReLu**
   <img alt="metrics" src="https://res.cloudinary.com/robertosousa1/image/upload/v1604366440/tcc/download_wt3jgk.png" width="520px" />
   <img alt="metrics" src="https://res.cloudinary.com/robertosousa1/image/upload/v1604366440/tcc/download_1_rl03eo.png" width="520px" />
   <img alt="metrics" src="https://res.cloudinary.com/robertosousa1/image/upload/v1604366440/tcc/download_2_uwzgbl.png" width="520px" />
   <img alt="metrics" src="https://res.cloudinary.com/robertosousa1/image/upload/v1604366440/tcc/Captura_de_Tela_2020-11-02_a%CC%80s_21.52.05_nafqwg.png" width="520px" />

	- Testamos diversas outras funções de ativação que se mostram compatível com o nosso modelo. Segue relação das funções testadas abaixo:
		- Sigmoid / Logistic
		- TanH
		- Elu
		- Leaky ReLU
		- Swish

## [](#license):memo: Licença
This project is under the MIT license. See the [LICENSE](https://github.com/robertosousa1/skin-cancer-detection/blob/master/LICENSE) for more information.
