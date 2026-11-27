## 1. Requisitos funcionais (RF)

### Gerenciamento de usuários e pacientes

| ID | Descrição |
| --- | --- |
| RF01 | Permitir o cadastro de usuários no sistema.  
| RF02 | Permitir que um usuário atue como paciente, cuidador ou ambos.  
| RF03 | Permitir que cuidadores cadastrem pacientes que não possuam conta própria.  
| RF04 | Permitir a vinculação de uma conta de usuário a um paciente previamente cadastrado, preservando seu histórico.  
| RF05 | Permitir que pacientes autorizem cuidadores a acompanharem seus tratamentos.  
| RF06 | Permitir que um paciente seja acompanhado por múltiplos cuidadores.  
| RF07 | Permitir que um cuidador acompanhe múltiplos pacientes.  
| RF08 | Permitir que cuidadores autorizados consultem todos os tratamentos dos pacientes acompanhados.  
| RF09 | Permitir a revogação de autorizações concedidas aos cuidadores, preservando os registros anteriormente realizados.  

### Gerenciamento de medicamentos

| ID | Descrição |
| --- | --- |
| RF10 | Disponibilizar um catálogo compartilhado de medicamentos.  
| RF11 | Permitir a inclusão de novos medicamentos no catálogo.  
| RF12 | Permitir a consulta aos medicamentos cadastrados.  

### Gerenciamento de tratamentos e prescrições

| ID | Descrição |
| --- | --- |
| RF13 | Permitir o registro de múltiplos tratamentos associados a um paciente.  
| RF14 | Permitir o registro de tratamentos com duração determinada ou indeterminada.  
| RF15 | Permitir o registro de uma ou mais prescrições associadas a um tratamento.  
| RF16 | Permitir que pacientes e cuidadores autorizados registrem prescrições.  
| RF17 | Permitir a associação de múltiplos medicamentos a uma prescrição.  
| RF18 | Permitir o registro da dosagem, frequência, horários e período de utilização de cada medicamento prescrito.  
| RF19 | Permitir o registro de alterações nas orientações recebidas dos profissionais de saúde para cada medicamento prescrito.  
| RF20 | Manter um histórico individual das alterações nas orientações de cada medicamento prescrito.  
| RF21 | Permitir o registro da interrupção de tratamentos, incluindo data, motivo e responsável pelo registro.  

### Gerenciamento de doses

| ID | Descrição |
| --- | --- |
| RF22 | Gerar antecipadamente as doses programadas com base nas orientações prescritas.  
| RF23 | Gerar e renovar periodicamente as doses dos tratamentos de duração indeterminada, considerando uma janela de sete dias.  
| RF24 | Permitir a consulta às doses programadas.  
| RF25 | Permitir que pacientes e cuidadores autorizados registrem a administração das doses.  
| RF26 | Identificar automaticamente as doses esquecidas após o período de tolerância estabelecido pelo sistema.  
| RF27 | Permitir o registro da administração de doses atrasadas, inclusive aquelas anteriormente identificadas como esquecidas.  
| RF28 | Registrar a data e o horário reais da administração de cada dose.  
| RF29 | Atualizar as doses futuras afetadas por alterações nas orientações prescritas, preservando o histórico dessas orientações.  
| RF30 | Permitir a consulta ao histórico de doses administradas e esquecidas.  

### Gerenciamento de lembretes

| ID | Descrição |
| --- | --- |
| RF31 | Emitir lembretes referentes às doses programadas.  
| RF32 | Permitir a configuração dos destinatários dos lembretes.  
| RF33 | Manter um histórico dos lembretes enviados.  

### Preservação do histórico 

| ID | Descrição |
| --- | --- |
| RF34 | Cancelar as doses futuras de tratamentos interrompidos, preservando seus registros.  
| RF35 | Identificar e registrar o usuário responsável pelo registro de cada administração de medicamento.  
| RF36 | Identificar e registrar o usuário responsável pelo registro de cada alteração nas orientações prescritas.  


## 2. Requisitos não funcionais (RNF)

| ID | Categoria | Descrição |
| --- | --- | --- |
| RNF01 | Segurança | Proteger os dados contra acessos e modificações não autorizados.  
| RNF02 | Privacidade | Restringir o acesso às informações dos pacientes aos usuários devidamente autorizados.  
| RNF03 | Integridade | Garantir a integridade referencial e a consistência das informações armazenadas.  
| RNF04 | Confiabilidade | Garantir que as operações de alteração dos dados não comprometam os registros existentes.  
| RNF05 | Rastreabilidade | Possibilitar a identificação dos responsáveis pelos registros cuja autoria deve ser preservada.  
| RNF06 | Manutenibilidade | Possuir uma estrutura de dados documentada e compreensível, facilitando sua manutenção e evolução.  