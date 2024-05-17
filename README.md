
# Repositório de Projetos do Modellus

Neste repositório, você encontrará uma lista de várias modelagens. Cada uma delas possui um título referente ao nome do arquivo, juntamente com uma descrição e um vídeo demonstrativo de seu funcionamento.

---
## Formação de Imagem em Espelhos - Foco(t)
[![Formação de Imagem em Espelhos - Foco(t)](https://img.youtube.com/vi/D-VqBdoeOPA/0.jpg)](https://youtu.be/D-VqBdoeOPA)
#### Introdução
https://youtu.be/D-VqBdoeOPA
Esta modelagem simula a formação de imagens em espelhos côncavos e convexos, mostrando como a posição do foco altera a imagem formada. A modelagem foi realizada no software Modellus, permitindo a manipulação dos parâmetros físicos e a observação do comportamento da imagem conforme o foco do espelho é alterado.

#### Descrição do Modelo

1. **Equações Fundamentais**

   - **Imagem (\(i\))**:
     \[
     i = \frac{f \cdot p}{p - f}
     \]
     Onde \(f\) é a distância focal e \(p\) é a posição do objeto.

   - **Altura da Imagem (\(h_i\))**:
     \[
     h_i = m \cdot h
     \]
     Onde \(h\) é a altura do objeto e \(m\) é o aumento linear.

   - **Aumento Linear (\(m\))**:
     \[
     m = \frac{-i}{p}
     \]

   - **Raio de Curvatura (\(r\))**:
     \[
     r = 2 \cdot f
     \]

2. **Interseções e Posições**

   - **Interseção do Raio Incidente Perpendicular (\(\text{interc\_x\_raio\_inci\_perpen}\))**:
     \[
     \text{interc\_x\_raio\_inci\_perpen} = \sqrt{(r^2) - (h^2)} + r
     \]

   - **Posição do Raio Incidente Perpendicular (\(x\_\text{raio\_inci\_perpen}\))**:
     \[
     x\_\text{raio\_inci\_perpen} = p - \text{interc\_x\_raio\_inci\_perpen}
     \]

   - **Foco Corrigido para o Raio Incidente 1 (\(f\_\text{corrigido\_to\_raio\_inc1}\))**:
     \[
     f\_\text{corrigido\_to\_raio\_inc1} = f - h
     \]

   - **Posição da Reta Incidente 1 (\(x\_\text{reta\_inc\_1}\))**:
     \[
     x\_\text{reta\_inc\_1} = f - \text{interc\_x\_raio\_inci\_perpen}
     \]

   - **Altura da Reta Incidente 1 (\(y\_\text{reta\_inc\_1}\))**:
     \[
     y\_\text{reta\_inc\_1} = 0 - h
     \]

3. **Parâmetros Iniciais**

   - A posição inicial do objeto (\(p\)) é definida como:
     \[
     p = -450
     \]

   - O foco do espelho (\(f\)) é atualizado a cada passo:
     \[
     f = \text{last}(f) + 1
     \]

#### Simulação

A simulação permite ajustar a posição do objeto (\(p\)), a altura do objeto (\(h\)), e o foco do espelho (\(f\)). Conforme o foco do espelho é alterado, ele pode mudar de côncavo para convexo, impactando a posição e o tamanho da imagem formada. Através do Modellus, é possível visualizar como a imagem se comporta em diferentes configurações do espelho.

#### Resultados Esperados

Dependendo da configuração do foco e da posição do objeto, a imagem formada pode variar entre real e virtual, direita e invertida, ampliada ou reduzida. Esta modelagem demonstra a importância do foco na formação de imagens em espelhos esféricos e permite uma compreensão visual clara dos princípios óticos envolvidos.

#### Conclusão

Este modelo, desenvolvido no Modellus, oferece uma ferramenta interativa para explorar a formação de imagens em espelhos côncavos e convexos. A capacidade de ajustar os parâmetros em tempo real proporciona uma análise detalhada e uma melhor compreensão dos conceitos óticos fundamentais.

## Formação de Imagem em Espelhos - Posição(t)
[![Formação de Imagem em Espelhos - Posição(t)](https://img.youtube.com/vi/q_VbTEQx18k/0.jpg)](https://www.youtube.com/watch?v=q_VbTEQx18k)

#### Introdução

Esta modelagem demonstra a relação entre imagem e objeto real. É possível ajustar todos os parâmetros físicos e observar como eles se comportam quando a posição do objeto é alterada ao longo de um espelho côncavo ou convexo.

#### Descrição do Modelo

É a mesma de Formação de Imagem em Espelhos - Foco(t)

#### Simulação

Nesta simulação, a posição do objeto depende do tempo e é incrementada conforme o tempo passa, permitindo observar o objeto se aproximando e atravessando o vidro. Isso demonstra o funcionamento de um espelho côncavo e convexo em uma única modelagem. Através do Modellus, é possível visualizar como a imagem se comporta à medida que a posição do objeto muda.

#### Resultados Esperados

Dependendo da posição do objeto e do tipo de espelho (côncavo ou convexo), a imagem formada pode variar entre real e virtual, direita e invertida, ampliada ou reduzida. Esta modelagem permite explorar a formação de imagens em diferentes posições do objeto e entender melhor os princípios óticos envolvidos.

#### Conclusão

Este modelo, desenvolvido no Modellus, oferece uma ferramenta interativa para explorar a formação de imagens em espelhos côncavos e convexos com a posição do objeto variando ao longo do tempo. A capacidade de ajustar os parâmetros em tempo real proporciona uma análise detalhada e uma melhor compreensão dos conceitos óticos fundamentais.

## Comportamento de Partículas em Campos Elétricos e Magnéticos
[![Comportamento de Partículas em Campos Elétricos e Magnéticos](https://img.youtube.com/vi/Cs4K8Rgw52k/0.jpg)](https://youtu.be/Cs4K8Rgw52k)

#### Introdução

Esta modelagem simula o comportamento de uma partícula carregada ao atravessar placas que geram um campo elétrico. O objetivo é estudar como a partícula é influenciada pelas forças elétricas e magnéticas e prever sua trajetória. A modelagem foi realizada utilizando o software Modellus, permitindo controlar parâmetros como a velocidade inicial da partícula, a carga da partícula e a intensidade dos campos elétrico e magnético.

#### Descrição do Modelo

1. **Forças Atuantes na Partícula**

   - **Força Elétrica (\(F_e\))**:
     \[
     F_e = |q| \cdot |E|
     \]
     Onde \(q\) é a carga da partícula e \(E\) é a magnitude do campo elétrico.

   - **Força Magnética (\(F_m\))**:
     \[
     F_m = -|B| \cdot |q| \cdot \text{Modl}_v
     \]
     Onde \(B\) é a magnitude do campo magnético e \(\text{Modl}_v\) é a magnitude da velocidade da partícula.

2. **Força Resultante (\(F_{\text{res}}\))**

   A força resultante na partícula é zero (\(F_{\text{res}} = 0\)) se a partícula estiver fora do alcance das placas. Dentro do campo elétrico gerado pelas placas, a força resultante é a soma das forças elétrica e magnética:
   \[
   F_{\text{res}} = F_e + F_m
   \]

3. **Equações de Movimento**

   - **Aceleração**:
     \[
     a_y = \frac{F_{\text{res}}}{m}
     \]
     Onde \(m\) é a massa da partícula e \(a_y\) é a aceleração no eixo \(y\).

   - **Velocidade**:
     \[
     v_x = \text{last}(v_x) + a_x \cdot \text{passo}
     \]
     \[
     v_y = \text{last}(v_y) + a_y \cdot \text{passo}
     \]
     Onde \(a_x\) e \(a_y\) são as componentes da aceleração, e \(\text{passo}\) é o intervalo de tempo entre cada cálculo.

   - **Posição**:
     \[
     p_x = \text{last}(p_x) + v_x \cdot \text{passo}
     \]
     \[
     p_y = \text{last}(p_y) + v_y \cdot \text{passo}
     \]
     Onde \(p_x\) e \(p_y\) são as coordenadas da posição da partícula.


#### Simulação

A simulação permite ajustar a velocidade inicial da partícula (\(v_x\), \(v_y\)), a carga (\(q\)), o campo elétrico (\(E\)), e o campo magnético (\(B\)). Através do Modellus, é possível visualizar a trajetória da partícula enquanto ela se move sob a influência das forças elétricas e magnéticas entre as placas.

#### Resultados Esperados

Dependendo dos parâmetros ajustados, a partícula pode:

- Acelerar ou desacelerar enquanto atravessa o campo elétrico.
- Desviar sua trajetória devido à força magnética.
- Manter uma velocidade constante se as forças se cancelarem perfeitamente.

A simulação demonstra a complexa interação entre os campos elétrico e magnético, proporcionando uma visualização clara de conceitos importantes na física de partículas carregadas.

#### Conclusão

Este modelo, desenvolvido no Modellus, oferece uma ferramenta poderosa para explorar e entender o comportamento das partículas carregadas em campos elétricos e magnéticos. A capacidade de ajustar os parâmetros em tempo real permite uma análise detalhada e uma melhor compreensão dos princípios físicos envolvidos.


