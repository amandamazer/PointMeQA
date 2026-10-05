LEIAME:
=======

O "Point Me QA" permite a identificação semi-automática de pontos de referência em imagens médicas 3D e 4D, os quais podem ser utilizados como referenciais para realizar registro de imagem, para validação de registro de imagem ou para quantificação de movimentação. Isso pode ser feito por usuários sem experiência, visando fornecer suporte acadêmico para o avanço das pesquisas na área de Radioterapia Guiada por Imagem (IGRT).

=========================
Para executar o programa:
1. Descompacte o arquivo baixado.
2. Na pasta "PointMeQA", dê dois cliques para executar o arquivo também de nome "PointMeQA".
3. Siga os passos de como utilizá-lo e verifique os arquivos gerados e salvos dentro dessa mesma pasta. 

==============
Como utilizar:
1. Informe o nome do paciente e a dimensão das imagens a serem utilizadas.
2. Através do botão 'Selecionar', localize o diretório geral que contém os diretórios das imagens e das estruturas de interesse dos pacientes.
3. Especifique por extenso o nome do diretório da imagem escolhida como referência, assim como a modalidade dela - CT ou CBCT.
4. Informe por extenso os nomes das segmentações de interesse que deseja utilizar, separados por vírgula. Essas segmentações serão utilizadas apenas como limitadoras de regiões para identificação dos pontos. Se deixado em branco, o algoritmo utiliza a imagem toda para extração.
5. Se forem imagens 3D, é possível especificar uma segunda imagem, escolhida como imagem móvel, se desejado. Selecione também se há transformação entre as duas imagens, resultantes de um registro, especificando o nome por extenso, que devem estar no diretório do paciente em formato .tfm. Caso seja uma imagem 4D, especifique o número das fases respiratórias de interesse para identificação, separadas por vírgula, sendo de 0 a 90, com passo de 10.
6. Selecione a(s) distância(s) de interesse que será utilizada como métrica para identificação dos pontos correspondentes entre as imagens.
7. Selecione em quais regiões da imagem os pontos devem ser identificados, se apenas de alto ou de alto e de baixo contraste.
8. Por fim, selecione as caixas de acordo com o interesse em: extrair os nomes das segmentações que acompanham as imagens para utilizá-las como limitadoras de região de interesse; gerar um relatório de análise utilizando os pontos de referência identificados; limitar a distância residual entre os pontos correspondentes, eliminando aqueles muito distantes e possivelmente de falsa correspondência; gerar os arquivos de coordenadas dos pontos de cada imagem compatível para leitura no software 3D Slicer; realizar análise de dose utilizando os pontos identificados, caso as imagens acompanhem distribuição de dose; e calcular a Informação Mútua (IM) entre as imagens fornecidas.
9. Clique no botão 'Iniciar' para executar o algoritmo. É comum que o programa apresente que não está respondendo enquanto é executado, no entanto, os resultados serão apresentados normalmente.
10. Após o término, selecione se deseja escolher quais pontos correspondentes manter — modo de extração semi-automático.
11. Terminada a execução, que pode durar minutos ou horas dependendo das imagens utilizadas, todos os arquivos resultantes estarão salvos no diretório deste executável.
12. Caso pretenda executar outro caso, feche e abra o executável novamente.

=========================
Este programa de computador foi registrado no Instituto Nacional da Propriedade Industrial (INPI) com processo de número BR512024000601-0.
Em caso de maiores dúvidas, é possível obter ajuda através do e-mail: amandamazer18@gmail.com

=========================
Como citar / referenciar:
MAZER, Amanda C. Desenvolvimento de um algoritmo para avaliação de registro de imagem em Radioterapia Guiada por Imagem (IGRT). 2024. Tese (Doutorado em Tecnologia Nuclear) – Instituto de Pesquisas Energéticas e Nucleares – IPEN-CNEN/SP. São Paulo.
