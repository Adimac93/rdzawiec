# Rdzawiec

![Logo](logo.png)

Aren't you _wkurwiony/a_ from writing Rust programs in English? Do you like saying
"kurwa" a lot? Would you like to try something different, in an exotic and
funny-sounding language? Would you want to bring some **Polish** to your
programs?

**rdzawiec** (Polish for __pollack__) is here to save your day, as it allows you to
write Rust programs in Polish, using Polish keywords, Polish function names,
Polish idioms.

This has been designed to be used as the official programming language to
develop the future Polish sovereign operating system.

You don't feel at ease using only Polish words? Don't worry!
Polish Rust is fully compatible with English-Rust, so you can mix both at your
convenience.

Here's an example of what can be achieved with Rdzawiec:

### trait and impl (aka cecha i implementacja)

```rust
rdzawiec::rdzawiec! {
    zewnętrzna skrzynka rdzawiec;

    użyj standardowe::kolekcje::MapaHaszy jako Mapa;

    cecha WartościPoKluczu {
        funkcja zapisz(&się, klucz: Ciąg, wartość: Ciąg);
        funkcja wczytaj(&się, klucz: Ciąg) -> Wynik<Opcja<&Ciąg>, Ciąg>;
    }

    statyczna zmienna SŁOWNIK: Opcja<Mapa<Ciąg, Ciąg>> = Żadna;

    struktura Słownik;

    implementacja WartościPoKluczu dla Słownik {
        funkcja zapisz(&się, klucz: Ciąg, wartość: Ciąg) {
            niech słownik = niebezpieczne {
                SŁOWNIK.wyjmij_lub_wstaw_z(Domyślny::domyślny)
            };
            słownik.wstaw(klucz, wartość);
        }
        funkcja wczytaj(&się, klucz: Ciąg) -> Wynik<Opcja<&Ciąg>, Ciąg> {
            jeżeli niech Jakiś(słownik) = niebezpieczne { SŁOWNIK.jako_referencja() } {
                Dobrze(słownik.wyjmij(&klucz))
            } inaczej {
                Źle("nie ma słownika".do())
            }
        }
    }
}
```

### Support for regional languages

```rust
#[pozwól(nieosiągalny_kod)]
funkcja druga() {
    kurwa!("zjebało się"); // for the true Polish experience
    jerōnie!("motyka"); // for friends speaking ślōnska gŏdka
    panikuj!("motyla noga"); // in SFW contexts
}
```

### Other examples

See the [examples](./examples/src/main.rs) to get a rough sense of the whole
syntax. Proszę, that's it.

## Kontrybucje

First of all, _dzięki wielkie_ for considering participating to this joke, the
Polish government will thank you later! Feel free to throw in a few identifiers
here and there, and open a pull-request against the `główna` (Polish for
`main`) branch.

## Other languages

- French (original): [rouille](https://github.com/bnjbvr/rouille)
- Dutch: [roest](https://github.com/jeroenhd/roest)
- German: [rost](https://github.com/michidk/rost)
- Italian: [ruggine](https://github.com/DamianX/ruggine)
- Russian: [Ржавый](https://github.com/Sanceilaks/rzhavchina)
- Esperanto: [rustteksto](https://github.com/dscottboggs/rustteksto)
- Hindi: [zung](https://github.com/rishit-khandelwal/zung)
- Hungarian: [rozsda](https://github.com/jozsefsallai/rozsda)
- Chinese: [xiu (锈)](https://github.com/lucifer1004/xiu)
- Spanish: [rustico](https://github.com/UltiRequiem/rustico)
- Korean: [Nok (녹)](https://github.com/Alfex4936/nok)
- Finnish: [ruoste](https://github.com/vkoskiv/ruoste)
- Arabic: [sada](https://github.com/LAYGATOR/sada)
- Turkish: [pas](https://github.com/ekimb/pas)
- Vietnamese: [gỉ](https://github.com/Huy-Ngo/gir)
- Japanese: [sabi (錆)](https://github.com/yuk1ty/sabi)
- Danish: [rust?](https://github.com/LunaTheFoxgirl/rust-dk)
- Marathi: [gan̄ja](https://github.com/pranavgade20/ganja)
- Romanian: [rugină](https://github.com/aionescu/rugina)
- Czech: [rez](https://github.com/radekvit/rez)
- Ukrainian: [irzha](https://github.com/brokeyourbike/irzha)
- Bulgarian: [ryzhda](https://github.com/gavadinov/ryzhda)
- Slovak: [hrdza](https://github.com/TheMessik/hrdza)
- Catalan: [rovell](https://github.com/gborobio73/rovell)
- Corsican: [rughjina](https://github.com/aldebaranzbradaradjan/rughjina)
- Indonesian: [karat](https://github.com/annurdien/karat)
- Lithuanian: [rūdys](https://github.com/TruncatedDinosour/rudys)
- Greek: [skouriasmeno](https://github.com/devlocalhost/skouriasmeno)
- Thai: [sanim (สนิม)](https://github.com/korewaChino/sanim)
- Swiss: [roeschti](https://github.com/Georg-code/roeschti)
- Swedish: [rost](https://github.com/vojd/rost/)
- Croatian: [hrđa](https://github.com/njelich/hrdja)
- Persian: [zangar (زنگار)](https://github.com/ui-ce/zangar)
- Malagasy: [arafesina](https://github.com/luckasRanarison/arafesina)
- Latin: [ferrugo](https://github.com/pianoman911/ferrugo)
- Norwegian: [korrosjon](https://github.com/datagutt/korrosjon)
- Estonian: [rooste](https://github.com/hanshs/rooste)
- All of the above: [unirust](https://github.com/charyan/unirust)

## Podziękowania

- [@bnjbvr](https://github.com/bnjbvr) for making the original macro.

## Licencja

[WTFPL](http://www.wtfpl.net/).
