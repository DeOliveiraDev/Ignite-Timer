## FORM
Controlled == é um formulário que é atualizado em tempo real a cada mudança nos campos (Usamos o onChange para captar essas mudanças e o value para captar mudanças de fora do input mas, que afetam o seu valor).

+ Controle
+ Ajuda a criarmos layouts onde habilitamos ou desabilitamos uma funcionalidade conforme o usuário digita ou apaga os valores em um input.

Uncontrolled == é um formulário no qual apenas obtemos os valores dos inputs quando necessário (Usamos o onSubmit para captar os valores dos inputs).

+ Performace (Pois a aplicação não precisa ficar se preocupando com as alterações de valores)

OBS: Não necessariamente um FORM Controlled prejudica a performace da aplicação mas, em alguns casos, pode vir a se tornar um problema.

## React Hook Form

npm i react-hook-form

É uma biblioteca que por de baixo dos panos utiliza os conceitos de controlled e uncontrolled.
Para manter a lib pequena, o React Hook Form não fornece validação para formulários mas, ele oferece integração com outras libs que fazem validação.
Para se realizar integrações com as libs de Validações é necessário instalar:

register = Adiciona as funções e muitas outras funcionalidades como onBlur, onChange e etc como propriedade em um input. (syntax: {...register('NOME_DO_INPUT')})

handleSubmit = Verifica se houve um submit no formulário é importante criar uma função que indica o que será feito ao se ter um submit e essa função precisa ser passada como parametro para o handleSubmit.

watch = Fica de olho em um input (Transforma o input em um controlled input)

formState = Dentro do formState é possível acessar os erros da aplicação. (formState.errors)

npm i @hook/resolvers

## Zod for Form Validation

npm i zod

## useEffect

Se você usar o useEffect muitas vezes para atualizar estados no react de forma sincrona, você pode estar usando o useEffect de forma errada.