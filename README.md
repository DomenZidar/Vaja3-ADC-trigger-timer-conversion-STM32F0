# Vaja3-ADC-trigger-timer-conversion-STM32F0
1.Glede na vašo razvojno ploščico in razširitveno vezje z tipkami ter potenciometri, izberite ustrezni analogni vhod. Kateri pin je to?

To je pin PC0.

2.Glede na potenciometer na vaši ploščici izberite-obkljukajte ustrezni kanal/pin. Na zaslonu se vam mora ustrezno pobarvati izbrani pin v zeleno barvo. Kaj se izpiše poleg pina?

Poleg pina se izpiše ADC_IN10.

3.Aktiviramo samo zeleno LED diodo na ustreznem izhodu PC9. 

4.V Clock Configuration spremenimo APB1 Timer clock (MHz) na 16 MHz. Kaj opazite?

Opazimo, da se APB1 peripheral clock nastavi na polovico APB Timer clock-a, drugi pa se nastavijo na isto frekvenco kot APB1 Timer clock.

5.V Configuration kliknemo ADC gumb za TIM1, ki je v polju Control. Časovniku bi radi spremenili frekvenco na 1 kHz, zato moramo frekvenco ABP1 Timer Clock preskalirati v polju Prescaler (PSC - 16 bit value). Koliko znaša ta vrednost?

Ta vrednost znaša 16000.

6.Branje vrednosti želimo prikazati z utripanjem zelene LED diode na STM32f0 ploščici. Uporabite metodo TogglePin iz HAL knjižnice in zapišite ukaz:

HAL_GPIO_TogglePin(GPIOC, GPIO_PIN_9); 

Komentar: 

Program deluje brez napak.
