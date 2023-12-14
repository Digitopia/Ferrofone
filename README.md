# Ferrofone

Ferrofone is an instrument and interactive installation that allows for the exploration of the relationship between sound, its surrounding environment, and the way it alters our sense of direction and awareness of the world around us.

It was inspired by the sound sculptures of the Baschet brothers, pioneer artists who worked with industrial materials like metals and plastics in order to create objects which are simultaneously musical instruments, sculptures and engineering works.

The sounds that are triggered on the interaction were recorded at Casa da Música, on January 2023, and were played by portuguese percussionist Nuno Aroso on a Baschet instrument which is part of Casa da Musica's instrument collection.

This package includes the Pure Data patch and samples used in its development.  
This was implemented using a Bela mini, although you can also use any other computer or system on a chip capable of running Pure Data.

---

#### Patch Description

The main patch is taking 2 inputs from piezo microphones located in two different places of the playing surface, feeding those two inputs into two separate instances of the bonk~ object. The time diference between the triggering of the two bonk~objects is being used to figure out the area of the playing surface which is being striked. The triggers from the two areas are being used to trigger two groups of samples of attacks from the original Baschet instrument.

The template feature of the bonk object is being used to train the bonk~ objects to ignore strikes on the surface of the instrument and respond mostly to strikes on the metal parts of the instrument. A training patch is provided, where it first learns 20 strikes of the surface to ignore, followed by 20 of the surfaces to respond to.

---

#### Team

- **Idea:** Óscar Rodrigues e Filipe Fernandes / Digitópia Casa da Música

- **Design and development:** Filipe Fernandes

- **Building:** Filipe Fernandes e Marcelo Reis

- **Development and buliding support:** Óscar Rodrigues, Miguel Bastos e Ricardo Vieira 

- **Sound Recording:** Daniel Santos

- **Baschet performer:** Nuno Aroso

- **Acknowledgments:** Francelino Fernandes (Fundipor)
