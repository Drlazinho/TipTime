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

### Atualização do App - Design e melhoria de experiência
- Aplicado conceito de Design de acordo com as <a href="https://developer.android.com/design?hl=pt-br">Diretrizes de Material Design</a>
- Melhorando a experiência do APP como:
    - Remover o teclado quando apertar o ENTER dentro do APP;
    - Girar o celular horizontal e verticalmente sem causar crash, cortes e outros defeitos;
    - Customizar o App ao  ativar o modo escuro pela configuração do celular;
 
 **Aprendizado e Dificuldades**
 - Já havia aplicado um função em que remover o teclado após dar o enter em um outro app, mas durante a leitura e prática da documentação do Android Studio, vi que tem um maneira mais ideal de aplica essa função, no entanto mais complexa.
    
        override fun private fun handleKeyEvent(view: View, keyCode: Int): Boolean {
        if (keyCode == KeyEvent.KEYCODE_ENTER) {
            // Hide the keyboard
            val inputMethodManager =
                getSystemService(Context.INPUT_METHOD_SERVICE) as InputMethodManager
            inputMethodManager.hideSoftInputFromWindow(view.windowToken, 0)
            return true
        }
        return false
**Resultado**

<img src="https://media.giphy.com/media/D0k1bta1yLiyBdjNeA/giphy.gif" width="480" height="226" >
<img src="https://media.giphy.com/media/jHAG4G4sV0z6BkjsbQ/giphy.gif" width="226" height="480" >




   

