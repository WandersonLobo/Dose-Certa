# Requisitos 

##  Requisitos funcionais (RF)

### Gerenciamento de usuários e pacientes

| ID | Descrição |
| --- | --- |
| RF01 | Permitir o cadastro de usuários no sistema. |
| RF02 | Permitir que um usuário atue como paciente, cuidador ou ambos. |
| RF03 | Permitir que pacientes concedam e revoguem autorizações de acompanhamento aos cuidadores. |
| RF04 | Permitir que pacientes e cuidadores autorizados consultem os respectivos tratamentos, prescrições e orientações prescritas. |

### Gerenciamento de medicamentos

| ID | Descrição |
| --- | --- |
| RF05 | Permitir o cadastro e a consulta de medicamentos em um catálogo compartilhado. |

### Gerenciamento de tratamentos e prescrições

| ID | Descrição |
| --- | --- |
| RF06 | Permitir o registro de tratamentos de duração determinada ou indeterminada associados a um paciente. |
| RF07 | Permitir que pacientes e cuidadores autorizados registrem prescrições associadas aos tratamentos. |
| RF08 | Permitir a associação de múltiplos medicamentos a uma prescrição por meio de itens prescritos. |
| RF09 | Permitir o registro da dosagem, frequência, horários e período de utilização de cada medicamento prescrito. |
| RF10 | Permitir o registro de alterações nas orientações prescritas, preservando seu histórico e identificando o usuário responsável. |
| RF11 | Permitir o registro da interrupção e da conclusão dos tratamentos. |

### Gerenciamento de doses

| ID | Descrição |
| --- | --- |
| RF12 | Gerar doses programadas com base nas orientações prescritas. |
| RF13 | Permitir a consulta às doses programadas. |
| RF14 | Permitir que pacientes e cuidadores autorizados registrem a administração das doses, incluindo administrações atrasadas, identificando a data, o horário real e o usuário responsável pelo registro. |
| RF15 | Identificar as doses esquecidas conforme o período de tolerância estabelecido pelo sistema. |
| RF16 | Atualizar ou cancelar doses futuras em decorrência de alterações nas orientações, interrupção ou conclusão dos tratamentos, preservando o histórico. |
| RF17 | Permitir a consulta ao histórico de doses administradas e esquecidas. |

### Gerenciamento de lembretes

| ID | Descrição |
| --- | --- |
| RF18 | Emitir lembretes aos pacientes referentes às doses programadas. |

##  Requisitos não funcionais (RNF)

| ID | Categoria | Descrição |
| --- | --- | --- |
| RNF01 | Segurança | Proteger os dados contra acessos e modificações não autorizados.  
| RNF02 | Privacidade | Restringir o acesso às informações dos pacientes aos usuários devidamente autorizados.  
| RNF03 | Integridade | Garantir a integridade referencial e a consistência das informações armazenadas.  
| RNF04 | Confiabilidade | Garantir que as operações de alteração dos dados não comprometam os registros existentes.  
| RNF05 | Rastreabilidade | Possibilitar a identificação dos responsáveis pelos registros cuja autoria deve ser preservada.  
| RNF06 | Manutenibilidade | Possuir uma estrutura de dados documentada e compreensível, facilitando sua manutenção e evolução.  