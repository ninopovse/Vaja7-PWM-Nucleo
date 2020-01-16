# Vaja7-PWM-Nucleo

# 2. Postopek inicializacijne periferije:

b) Prvi kanal aktivirajte kot PWM Generation CH1. Kateri pin ste omogočili? PA8. Kaj se izpiše poleg pina? TIM1_CH1

d) Koliko je vrednost Prescaler? 16

e) Koliko znaša sedaj?

# 3. Programiranje v SW4

c) Poiščite prenastavljeni parameter Pulse (ki je 50) v vaši kodi in pripišite ukaz, ki ga je generiral CubeMX:
   sConfigOC.Pulse = 50;

# 5. Dodatne nastavitve kode v programu SW4:

a)V kodi spremenite vrednost širine pulza na 25%. Zapišite popravljeni ukaz v kodi:
  sConfigOC.Pulse = 25;

Zapišite kaj počnejo ukazi v 1.,2. in 3. vrstici (v user code begin 3):

1. Na začetku zanke program nastavi htim1.Instance->CCR1 na vrednost spremenljivke dutyCycle.
2. V tej vrstici se dutyCycle vedno poveča za 10.
3. Če je dutyCycle večji od 90, se spremeni na 10 in tako nastane neskončna zanka.

# Komentar

S programom nastavljamo hitrost frekvence in širino pulza. S to vajo nisva imela nobenih težav.           
