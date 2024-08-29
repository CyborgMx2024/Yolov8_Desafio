O YOLOv8 é a versão mais recente da série de modelos YOLO (You Only Look Once), que são conhecidos por sua alta eficiência em detecção de objetos em tempo real. Assim como suas versões anteriores, o YOLOv8 continua focado em velocidade e precisão, mas traz várias melhorias significativas.

### Principais características do YOLOv8:
1. **Arquitetura Atualizada:** O YOLOv8 apresenta uma nova arquitetura de rede neural, otimizando ainda mais o equilíbrio entre velocidade e precisão.

2. **Melhorias em Treinamento:** Inclui técnicas de treinamento aprimoradas, como melhores estratégias de otimização, o que resulta em um treinamento mais eficiente e modelos mais robustos.

3. **Suporte a Tarefas Múltiplas:** Além da detecção de objetos, o YOLOv8 também suporta segmentação de instâncias e detecção de poses, ampliando suas capacidades.

4. **Facilidade de Uso:** A interface do YOLOv8 é projetada para ser mais amigável, facilitando a implementação e personalização, especialmente para usuários com menos experiência.

5. **Otimização para Inferência:** O YOLOv8 é altamente otimizado para uso em dispositivos com recursos limitados, como dispositivos móveis e embarcados, mantendo a eficiência em tempo real.

Em resumo, o YOLOv8 continua a tradição de seus antecessores, oferecendo um modelo rápido e preciso, mas com melhorias substanciais em desempenho e versatilidade para diferentes aplicações de visão computacional.

# Detecção e segmentação

!pip install ultralytics 
from ultralytics import YOLO  

#!yolo task=detect mode=predict model=yolov8n.pt  source="/content/robo.jpeg" save=True imgsz=320 conf=0.5

!yolo task=segment mode=predict model=/content/yolov8n-seg.pt  source="/content/pessoas.jpg" save=True imgsz=320 conf=0.5

from IPython.display import Image
Image('/content/runs/segment/predict2/pessoas.jpg')
