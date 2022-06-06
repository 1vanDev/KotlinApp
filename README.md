class MainActivity : AppCompatActivity() {
    lateinit var bindingClass: ActivityMainBinding
    val maxPerson = 90
    val currentPerson = 95

    override fun onCreate(s: Bundle?) {
        super.onCreate(s)
        bindingClass = ActivityMainBinding.inflate(layoutInflater)
        setContentView(bindingClass.root)

        bindingClass.B1.setOnClickListener  {
            if (maxPerson > currentPerson) {
            bindingClass.tvResult.text = ("Все в порядке")
            bindingClass.tvResult.setBackgroundColor(Color.GREEN)
            }

            else    {
            bindingClass.tvResult.text = ("Превышено количество посетителей")
            bindingClass.tvResult.setBackgroundColor(Color.RED)
            }

        bindingClass.B2.setOnClickListener {
        }

        bindingClass.B3.setOnClickListener {
        }

    }
}
}
