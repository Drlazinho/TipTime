## App TipTime (Hora da Gorjeta) com Kotlin 💸
Aplicativo desenvolvido através do Curso Lição 2 do Android Studio, um app que calcular o valor da gorjeta, tendo a opção da porcentagem e de arrendodamento do valor que quer ser pago.

**Aprendizado e Dificuldades**
- `Android.Kotlin.extensions` está sendo descontinuada, substituido pelo recurso de Vínculo de Visualizações `viewBinding`, fazendo ficar mais rápido a execução do app durante a visualização.
- Debugs, fazer que o app não quebre quando usuário deixa um valor nulo ou vazia.
- Entender a importância de nomeia os elementos da UI
- Refatoração do código, deixando o código menor, adotando boas práticas da programação
    
        lateinit var binding: ActivityMainBinding
    
        override fun onCreate(savedInstanceState: Bundle?) {
            super.onCreate(savedInstanceState)
            binding = ActivityMainBinding.inflate(layoutInflater)
            setContentView(binding.root)
        }
**Resultado**

<img src="https://media.giphy.com/media/gWWdcncsiXt5DHwdcW/giphy.gif" width="226" height="480" >
