# MIC1 - A Unidade Lógica e Aritmética

**Disciplina:** G05LAOC1.02 - Laboratório de Arquitetura e Organização de Computadores I  
**Repositório:** https://github.com/Jade-Souza/Mic1

## Integrantes

- Jade Giulia Januaria de Souza
- Otavio Vieira de Souza
- Kairo Henrique Ferreira Martins

## Arquivos do projeto (MIC1.qpf)

| Componente | Arquivos |
|---|---|
| Decodificador 2→4 | `DECODER_2TO4.bdf`, `.bsf`, `.vwf` |
| Full Adder 1 bit | `Full_Adder_1bit.bdf`, `.bsf`, `.vwf` |
| ULA 1 bit | `ULA_1bit.bdf`, `.bsf`, `.vwf`, `ULA_1bit_2.vwf` |
| ULA 8 bits | `ULA_8bits.bdf`, `.bsf`, `.vwf`, `ULA_8bits_2.vwf`, `ULA_8bits_3.vwf`, `ULA_8bits_4.vwf` |
| ULA 32 bits | `ULA_32bits.bdf`, `.bsf`, `.vwf` |

## Como simular (Quartus II 13.0)

1. Abrir `MIC1.qpf`
2. **Assignments → Settings → Simulator** → escolher **Quartus II Simulator**
3. Definir o top-level e o `.vwf` de entrada conforme o teste:
   - `ULA_1bit` + `ULA_1bit.vwf` (A AND B, A OR B, INV B, A+B)
   - `ULA_1bit` + `ULA_1bit_2.vwf` (ENA, ENB, INVA)
   - `ULA_8bits` + `ULA_8bits.vwf` … `ULA_8bits_4.vwf`
   - `ULA_32bits` + `ULA_32bits.vwf`
4. **Processing → Start Compilation**
5. **Processing → Start Simulation**
6. Conferir o resultado em `simulation/qsim/MIC1.sim.vwf`

## Validação

Arquivos de referência: https://github.com/christianherrera77/ALU_VALIDATION

## Entrega no SIGAA

Responder a atividade com o link deste repositório GitHub e os nomes dos integrantes acima.
