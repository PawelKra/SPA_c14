<template>
  <div class="container">
    <ul class="qmenu">
      <li @click="scrollToElem('o-laboratorium')">
        <span v-if="lindex !== 0">O Laboratorium</span>
        <span v-else>About Laboratory</span>
      </li>
      <li @click="scrollToElem('o-datowanie-dendro')">
        <span v-if="lindex !== 0">Datowanie Dendrochronologiczne</span>
        <span v-else>Dendrochronological Dating</span>
      </li>
      <li @click="scrollToElem('o-datowanie-rad')">
        <span v-if="lindex !== 0">Datowanie Radiowęglowe</span>
        <span v-else>Radiocarbon Dating</span>
      </li>
      <li @click="scrollToElem('o-kalibracja')">
        <span v-if="lindex !== 0">Kalibracja</span>
        <span v-else>Calibration</span>
      </li>
      <li @click="scrollToElem('o-info')">
        <span v-if="lindex !== 0">Informacje dla zleceniodawców</span>
        <span v-else>Requirements and Price offer</span>
      </li>
      <li @click="scrollToElem('o-kontakt')">
        <span v-if="lindex !== 0">Kontakt</span>
        <span v-else>Contact</span>
      </li>
    </ul>
  </div>

  <div class="container under-line mt-6 o-laboratorium" v-if="lindex !== 0">
    <h1 class="title">O Laboratorium</h1>
    <div class="columns is-vcentered mt-6">
      <div class="column is-5 lab-desc">
        <div class="block">
          Laboratorium oferuje datowanie radiowęglowe techniką scyntylacyjną.
          Jest wyposażone w spektrometr niskotłowy nowej generacji (3
          fotopowielacze) produkcji fińskiej –
          <strong>HIDEX 300SL</strong>, ultraniskotłowy spektrometr
          <strong>Quantulus 1220</strong> oraz prototypowy spektrometr
          skonstruowany na uniwersytecie w Reykjaviku – <strong>ICELS</strong>.
          Do uzyskiwania benzenu z próbek organicznych wykorzystywana jest linia
          preparacyjna o wydajności około <strong>1200 sztuk rocznie</strong>.
        </div>
        <div class="block">
          Laboratorium specjalizuje się w datowaniu próbek drewna i węgli
          drzewnych, szczególnie z wykorzystaniem metody dopasowania do krzywej
          kalibracyjnej (wiggle matching). Laboratorium można zlecić również
          datowanie wszystkich typów próbek standardowo analizowanych techniką
          konwencjonalną (patrz wymagane masy próbek).
        </div>
      </div>

      <div class="column">
        <div class="columns is-center">
          <figure class="image">
            <img src="/img/main.png" />
          </figure>
        </div>
      </div>
    </div>
  </div>

  <div class="container under-line mt-6 o-laboratorium" v-if="lindex !== 1">
    <h1 class="title">About Laboratory</h1>
    <div class="columns is-vcentered mt-6">
      <div class="column is-5 lab-desc">
        <div class="block">
          The laboratory offers radiocarbon dating with the scintillation
          technique. It is equipped with <strong> HIDEX 300SL</strong>, a
          low-background spectrometer of new generation (3 photomultipliers),
          produced in Finland, and purchased in December 2008. The benzene is
          extracted from organic samples in a preparation line of a capacity of
          about <strong>1200 samples per year</strong>.
        </div>
        <div class="block">
          The laboratory specialises in dating samples of wood and charcoals, in
          particular with the method of fitting the calibration curve (wiggle
          matching). It is also possible to commission to the laboratory dating
          of all types of samples analysed with the standard, conventional
          technology (look at the required weights of samples).
        </div>
      </div>
      <div class="column">
        <div class="columns is-center">
          <figure class="image">
            <img src="/img/main.png" />
          </figure>
        </div>
      </div>
    </div>
  </div>

  <div class="container under-line mt-6 o-datowanie-dendro" v-if="lindex !== 0">
    <div class="go-top" @click="goToBegin">^</div>
    <h1 class="title">Datowanie Dendrochronologiczne</h1>
    <div class="columns v-centered">
      <div class="column lab-desc is-5">
        <div class="block">
          Metodą dendrochronologiczną można datować próbki drewna, które na
          przekroju poprzecznym posiadają widoczne minimum 50 przyrostów
          rocznych. W przypadku gdy zachowały się zewnętrzne warstwy (biel, słój
          podkorowy) możliwe jest określenie wieku ścięcia drzewa z dokładnością
          do pory roku. Gatunkami charakteryzującymi się najlepszymi efektami
          datowania są jodła, sosna, świerk, dąb, jesion.
        </div>
        <div class="block">
          W laboratorium stosujemy zarówno metody pomiaru bezpośredniego prób
          drewna na urządzeniu autorskiej konstrukcji o dokładności pomiaru
          1/100 mm. W przypadku gdy nie ma możliwości pobrania wystarczającej
          wielkości próbki, pomiar wykonujemy na pozyskanych
          zortorektyfikowanych zobrazowaniach, przy minimalnej ingerencji w
          badany obiekt.
        </div>
      </div>
      <div class="column">
        <div class="block">
          <strong class="marg">Obiekty archeologiczne</strong>
          <p>
            Do poprawnego wydatowania obiektu archeologicznego niezbedne jest
            pobranie przynajmniej dziesięciu próbek, przy założeniu, że badana
            konstrukcja jest jednofazowa. Gdy zachodzi podejrzenie, że
            poszczególne fragmenty są różnowiekowe, prób do analizy należy
            pobrać więcej aby uzyskane datowanie było rzetelne.
          </p>
        </div>

        <div class="block">
          <strong class="marg">Obiekty architektoniczne, więźby dachowe</strong>
          <p>
            Specjalizujemy się w datowaniu budynków drewnianych, jak również
            więźb dachowych. Pracujemy na terenie całej Polski oraz w Europie
            wschodniej. Posiadamy niezbędny sprzęt i doświadczenie niezbędne do
            pobrania materiałów do badań w sposób mało inwazyjny.
          </p>
        </div>

        <div class="block">
          <strong class="marg">Obrazy, instrumenty muzyczne, rzeźby</strong>
          <p>
            Datowanie tak delikatnych i cennych przedmiotów jest skomplikowane i
            czasochłonne, a czasami niemożliwe do wykonania metodą
            dendrochronologiczną. Wykonaliśmy wiele datowań cennych dzieł sztuki
            oraz pobieramy/doradzamy jak w sposób najmniej inwazyjny pobrać
            materiał do badań.
          </p>
        </div>

        <div class="block show-more">
          <span class="important-text">Zwróć uwagę</span>
          <strong class="marg">Wielkość próbek do pomiaru</strong>
          <p>
            Pomiar wykonywany jest na przekroju poprzecznym przez drewno. Przy
            pobieraniu próbki należy zwócić uwagę aby pozyskany fragment
            zawierał jak najwięcej niezaburzonych przyrostów rocznych. Próbka na
            czas transportu powinna być zabezpieczona przed wysuszeniem.
            Wysokość próbki nie powinna przekraczać 10 cm.
          </p>
        </div>
      </div>
    </div>
  </div>

  <div class="container under-line mt-6 o-datowanie-dendro" v-if="lindex !== 1">
    <div class="go-top" @click="goToBegin">^</div>
    <h1 class="title">Dendrochronological Dating</h1>
    <div class="columns v-centered">
      <div class="column lab-desc is-5">
        <div class="block">
          Woden samples with at last 50 annual rings can be dated by
          dendrochronology method. In case sample has sapwood or bark there is
          posibilty to determine cutting down the tree to season in current
          year. Tree species that get best results are: fir, pine, spruce, oak
          and ash.
        </div>
        <div class="block">
          Most of samples are measured on device constructed in our lab with
          precision 1/100 mm. If wooden item can not be damaged, we performe
          measurements on ortorectified photos taken on places with minimal
          interference.
        </div>
      </div>
      <div class="column">
        <div class="block">
          <strong class="marg">Archeological sites</strong>
          <p>
            Correct dating of archeological site needs at least ten samples with
            assumption that construction is single-phase. If there is
            possibility of wide timespan modifications, more samples should be
            collected for analysis, if dating should be accurate.
          </p>
        </div>

        <div class="block">
          <strong class="marg">Architecture, roof truss</strong>
          <p>
            We specialise in wooden architecture, and buildings. We work in all
            Poland and Eastern Europe. We have all neccesary equipment and
            experience for collecting samples with very little invasion on
            analyzed object.
          </p>
        </div>

        <div class="block">
          <strong class="marg"
            >Paintings, wooden musical instruments, sculptures</strong
          >
          <p>
            Dating of declicate and presious objects is complicated and
            timeconsuming and sometimes impossible to end with succes by
            dendrochronological dating. W perform dating of many precious work
            of art making as less damage as possible to objects
          </p>
        </div>

        <div class="block show-more">
          <span class="important-text">Caution</span>
          <strong class="marg">Samples size</strong>
          <p>
            Measurements taking place on cross-section by tree. Durring aquiring
            sample You should choose fragment with as many as possible tree
            rings with no deformations. Sample should be protect from drying out
            and any mechanical damages. Height of sample should not exceed 10 cm
            (3-4 in).
          </p>
        </div>
      </div>
    </div>
  </div>

  <div class="container under-line mt-6 o-datowanie-rad" v-if="lindex !== 0">
    <div class="go-top" @click="goToBegin">^</div>
    <h1 class="title">Datowanie Radiowęglowe</h1>
    <div class="columns">
      <div class="column is-5">
        <div class="block lab-desc mt-6">
          Metodą <sup>14</sup>C datować można najróżniejsze materiały, których
          czasami nawet nie podejrzewalibyśmy o to, że zawierają węgiel. Na
          stronie internetowej Laboratorium w Waikato (Nowa Zelandia), znaleźć
          można imponująco długą listę materiałów: węgiel drzewny, drewno,
          gałązki, ziarna, kości, muszle morskie, rzeczne, z ujść rzek, skóra,
          torf, koprolity, osady z dna jezior, gyttja, gleba, lód z wierceń,
          pyłek roślin, włosy, ceramika, rudy metali, malowidła naścienne, stal,
          meteoryty, jaja ptasie, koralowce, otwornice, nacieki jaskiniowe,
          tufy, ślady krwi, tkaniny, papier, pergamin, szczątki ryb, szczątki
          owadów, żywice, kleje, poroża, rogi, woda.
        </div>
        <div class="block lab-desc">
          Możliwość pomiaru wieku nietypowych materiałów należy konsultować z
          Laboratorium. Niżej omówione są pokrótce typowe materiały.
        </div>
      </div>

      <div class="column">
        <div class="block">
          <strong class="marg"
            >Drewno, węgle drzewne, nasiona i inne roślinne szczątki
            makroskopowe</strong
          >
          <p>
            Te materiały są raczej odporne na zanieczyszczenia. Bardzo dobrze
            nadają się one do datowania. Celowe zwykle jest botaniczne
            rozpoznanie gatunku lub rodzaju rośliny. Rozpoznanie gatunku ważne
            jest dla uniknięcia roślin żyjących w środowisku wodnym (chodzi o
            „efekt rezerwuarowy”). Typowymi roślinnymi szczątkami makroskopowymi
            wykorzystywanymi do datowania, poza węglami drzewnymi i ziarniakami
            zbóż są owoce i inne nasiona, np. orzeszki brzóz, czy inne organy
            roślin, jak łuski brzóz, łodyżki mchów, albo fragmenty tkanek, np.
            peryderma.
          </p>
        </div>

        <div class="block">
          <strong class="marg">Kości</strong>
          <p>
            Pomiarowi wieku podlega tu kolagen wydzielony z kości. Kolagen jest
            względnie trwałą substancją, nie wymieniającą węgla z otoczeniem w
            trakcie zalegania kości w ziemi. Jednak laboratoryjna preparatyka
            kości jest trudna i czasochłonna. Wydzielenie kolagenu, którego może
            być bardzo mało, wymaga zastosowania specjalnych procedur.
            Najprostszym kryterium oceny stanu zachowania kolagenu jest jego
            zawartość w kości.
          </p>
        </div>

        <div class="block">
          <strong class="marg">Muszle</strong>
          <p>
            Muszle mięczaków wodnych, zwłaszcza jeziornych niezbyt nadają się do
            pomiaru wieku. Ze względu na dużą różnorodność źródeł węgla, z
            których czerpią organizmy, spodziewać się można dużego postarzenia.
          </p>
        </div>

        <div class="block show-more">
          <span class="important-text">Zwróć uwagę</span>
          <strong class="marg"
            >Wielkość obiektów do pomiaru (masa próbek)</strong
          >
          <p>
            Pomiarowi podlega węgiel, a różne substancje czy obiekty maja różne
            koncentracje węgla, zawierają go mniej lub więcej. Dlatego, w
            zależności od rodzaju materiału konieczne masy próbek będą różne.
          </p>
        </div>

        <i
          >Źródło: A. Walanus, T. Goslar Datowanie radiowęglowe, Wydawnictwo AGH
          Kraków 2010</i
        >
      </div>
    </div>
  </div>

  <div class="container under-line mt-6 o-datowanie-rad" v-if="lindex !== 1">
    <div class="go-top" @click="goToBegin">^</div>
    <h1 class="title">Radiocarbon Dating</h1>
    <div class="columns">
      <div class="column is-5">
        <div class="block lab-desc mt-6">
          After ‘Radiocarbon Dating’ by Walanus & Goslar: With the
          <sup>14</sup>C method it is possible to date the most various
          materials, of which sometimes we would not even suspect the fact that
          they contain carbon. In the website of the Waikato Laboratory (New
          Zealand) one may find impressively long list of materials: charcoal,
          wood, branches and twigs, grains, bones, sea and river shells, skin,
          peat, coprolites, bottom lake deposits, gyttja, soil, ice from
          drillings, plant pollen, hair, ceramics, metal ores, wall paintings,
          steel, meteorites, bird eggs, corals, foraminifers, cave
          incrustations, tuffs, blood traces, tissue, paper, parchment, remains
          of fish, insects, resin, glue, antlers, horns, water. Possibilities of
          the age measurement of non-typical materials should be consulted with
          the Laboratory. Typical materials are briefly discussed below.
        </div>
      </div>

      <div class="column">
        <div class="block">
          <strong class="marg"
            >Wood, charcoals, plant seeds and other macroscopic plant remains
          </strong>
          <p>
            These materials are rather resistant to pollution. They are very
            good for dating. Botanical determination of the plant species or
            genus is usually desirable. The recognition of the species is
            important for avoiding plants living in the aqueous environment (it
            concerns ‘the reservoir effect’). Typical macroscopic plant remains
            used for dating, except charcoals and cereal seeds, are fruits and
            other seeds, e.g. birch nuts, or various plant organs, as birch
            hulls, stalks of mosses, or tissue fragments, e.g. periderma.
          </p>
        </div>

        <div class="block">
          <strong class="marg">Bones</strong>
          <p>
            It is the collagen distinguished from the bones that is the subject
            of the age measurement. The collagen is a relatively long-lasting
            substance, not exchanging carbon with the surroundings during lying
            of the bones in the soil. However, laboratory preparation of the
            bones is difficult and time-consuming. Separation of the collagen,
            which may be present in very small quantities, requires application
            of special procedures. The simplest criterion of the assessment of
            the state of preservation of the collagen is its content in the
            bone.
          </p>
        </div>

        <div class="block">
          <strong class="marg">Shells</strong>
          <p>
            Shells of aqueous molluscs, especially the lake species, are not
            fitted to the age measurement. On the account of high diversity of
            the carbon sources, from which the organisms are taking this
            element, relatively high ageing would be possible.
          </p>
        </div>

        <div class="block show-more">
          <span class="important-text">Caution</span>
          <strong class="marg">
            Weight and dimensions of the objects for the measurement (mass of
            samples)
          </strong>
          <p>
            The subject of the measurements is carbon and various substances or
            objects may contain different amounts of this elements; the carbon
            concentrations may be higher or lower. Therefore, depending on the
            kind of material, the required masses of samples are different.
          </p>
        </div>

        <i>
          Ref: A. Walanus, T. Goslar Datowanie radiowęglowe, Wydawnictwo AGH
          Kraków 2010
        </i>
      </div>
    </div>
  </div>

  <div class="container under-line mt-6 o-kalibracja" v-if="lindex !== 0">
    <div class="go-top" @click="goToBegin">^</div>
    <h1 class="title">Kalibracja</h1>
    <div class="columns">
      <div class="column is-5">
        <div class="block lab-desc">
          Określenie zależności pomiędzy konwencjonalnym wiekiem radiowęglowym a
          wiekiem kalendarzowym jest przedmiotem kalibracji radiowęglowej skali
          czasu. Kalibracji dokonujemy na podstawie krzywej kalibracyjnej
          wyznaczonej w oparciu o pomiary <sup>14</sup>C próbek o znanym wieku
          (głównie dendrochronologicznie datowanych słojach drzew). Otrzymany w
          efekcie kalibracji tzw. wiek kalibrowany jest najlepszym przybliżeniem
          kalendarzowego wieku próbki. Wiek kalibrowany podaje się jako
          przedział, który z prawdopodobieństwem 95% (lub 68%) zawiera wiek
          kalendarzowy próbki.
        </div>
      </div>
    </div>
  </div>

  <div class="container under-line mt-6 o-kalibracja" v-if="lindex === 0">
    <div class="go-top" @click="goToBegin">^</div>
    <h1 class="title">Calibration</h1>
    <div class="columns">
      <div class="column is-5">
        <div class="block lab-desc">
          Determination of the relation between the conventional radiocarbon age
          and the calendar age is the object of the calibration of the
          radiocarbon scale of time. The calibration is made on the basis of the
          calibration curve outlined by the <sup>14</sup> measurements of
          samples of a known age (mainly tree rings dated
          dendrochronologically). The so-called calibrated age, produced from
          the calibration, is the best approximation of the calendar age of the
          sample. The calibrated age is given as a range, which contains the
          calendar age of the sample with the probability of 95% (or 68%).
        </div>
      </div>
    </div>
  </div>

  <div class="container under-line mt-6 o-info" v-if="lindex !== 0">
    <div class="go-top" @click="goToBegin">^</div>
    <h1 class="title">Informacje dla zleceniodawców</h1>
    <div class="columns is-vcentered">
      <div class="column is-5">
        <h2 class="subtitle">CENNIK</h2>
        <div class="block lab-desc">
          Usługa datowania obejmuje preparatykę próbki, pomiar koncentracji
          <sup>14</sup>C techniką scyntylacyjną, podanie konwencjonalnego wieku
          radiowęglowego oraz daty kalibrowanej (w formie wykresu i zestawu
          zakresów wieku, przy różnych opcjach). <br />
          <br />
          Przesłanym próbkom do datowania powinno towarzyszyć zlecenie z danymi
          do faktury oraz opisy próbek na formularzach LBD.
          <br />
          <br />
          <p class="block">
            Do pobrania:<br /><br />
            <a href="/files/Formularz_LBD2015.pdf" target="_blank"
              ><img src="/img/pdficon_small.gif" width="16" height="16"
            /></a>
            <a href="/files/Formularz_LBD2015.pdf" target="_blank"
              >Formularz LBD (PDF)</a
            >
            <br />
            <a href="/files/Formularz_LBD.doc" target="_blank"
              ><img src="/img/wordicon.gif" width="16" height="16"
            /></a>
            <a href="/files/Formularz_LBD2015.doc" target="_blank"
              >Formularz LBD (WORD)</a
            >
          </p>

          <p>
            Cena datowania radiowęglowego: <br />
            <strong class="marg">575 PLN </strong> za próbkę + 23% VAT
          </p>
          <p>
            Cena datowania dendrochronologicznego: <br />
            <strong class="marg">500 PLN </strong> za próbkę + 23% VAT
          </p>
        </div>

        <div class="block">
          <strong class="marg">Zniżki</strong>
          <br />
          Możliwe są indywidualnie negocjowane zniżki dla stałych zleceniodawców
          i przy większych zleceniach.
        </div>
      </div>

      <div class="column">
        <h2 class="subtitle">WYMAGANE MASY PRÓBEK</h2>
        <table class="table">
          <thead>
            <tr>
              <th>Materiał próbki</th>
              <th>Sugerowana masa próbki</th>
              <th>Min. masa próbki</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Drewno</td>
              <td>10-50 g</td>
              <td>2-5 g</td>
            </tr>
            <tr>
              <td>Węgiel drzewny</td>
              <td>5-30 g</td>
              <td>1-3 g</td>
            </tr>
            <tr>
              <td>Torf drzewny</td>
              <td>50-100 g</td>
              <td>2 g</td>
            </tr>
            <tr>
              <td>Kości</td>
              <td>200-300 g</td>
              <td>1-3 g</td>
            </tr>
            <tr>
              <td>Osady organiczne/gleby</td>
              <td>500 g</td>
              <td>100 g</td>
            </tr>
          </tbody>
        </table>

        <h2 class="subtitle">
          DOKŁADNOŚCI WIEKU KONWENCJONALNEGO W ZALEŻNOŚCI OD ZAKRESU WIEKU I
          WIELKOŚCI PRÓBEK
        </h2>
        <div class="block">
          <table class="table">
            <thead>
              <tr>
                <th>Wiek</th>
                <th>Optymalna wielkość próbki</th>
                <th>Minimalna wielkość próbki</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>500 BP</td>
                <td>40 lat</td>
                <td>60 lat</td>
              </tr>
              <tr>
                <td>1000 BP</td>
                <td>50 lat</td>
                <td>70 lat</td>
              </tr>
              <tr>
                <td>5000 BP</td>
                <td>60 lat</td>
                <td>90 lat</td>
              </tr>
              <tr>
                <td>10000 BP</td>
                <td>70-90 lat</td>
                <td>100-120 lat</td>
              </tr>
              <tr>
                <td>20000 BP</td>
                <td>150-200 lat</td>
                <td>250-300 lat</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
  </div>

  <div class="container under-line mt-6 o-info" v-if="lindex === 0">
    <div class="go-top" @click="goToBegin">^</div>
    <h1 class="title">Requirements & Price offer</h1>
    <div class="columns is-vcentered">
      <div class="column is-5">
        <h2 class="subtitle">PRICES</h2>
        <div class="block lab-desc">
          The dating encompasses: sample preparation, <sup>14</sup>C
          concentration measurements with the scintillation technique,
          determination of the conventional radiocarbon age and the calibrated
          date (in a graphical form and a set of the age ranges, at various
          options).
          <br />
          <br />
          The sample sent for the <sup>14</sup>C dating should be accompanied by
          an order with data for the invoice and a sample description in the LBD
          form.
          <br />
          <br />
          <p class="block">
            Download:<br /><br />
            <a href="/files/Formularz_LBD2015.pdf" target="_blank"
              ><img src="/img/pdficon_small.gif" width="16" height="16"
            /></a>
            <a href="/files/Formularz_LBD2015.pdf" target="_blank"
              >Form LBD (PDF)</a
            >
            <br />
            <a href="/files/Formularz_LBD.doc" target="_blank"
              ><img src="/img/wordicon.gif" width="16" height="16"
            /></a>
            <a href="/files/Formularz_LBD2015.doc" target="_blank"
              >Form LBD (WORD)</a
            >
          </p>

          <p>
            Price of radiocarbon dating: <br />
            <strong class="marg">575 PLN </strong> (ca 130€) per sample + 23%
            VAT
          </p>
          <p>
            Price of dendrochronology dating: <br />
            <strong class="marg">500 PLN </strong> (ca 125€) per sample + 23%
            VAT
          </p>
        </div>

        <div class="block">
          <strong class="marg">Discounts</strong>
          <br />
          Discounts individually negotiated, for permanent customers are also
          possible.
        </div>
      </div>

      <div class="column">
        <h2 class="subtitle">REQUIRED WEIGHTS OF SAMPLES</h2>
        <table class="table">
          <thead>
            <tr>
              <th>Sample material</th>
              <th>Suggested mass of sample</th>
              <th>Minimal mass of sample</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Wood</td>
              <td>10-50 g</td>
              <td>2-5 g</td>
            </tr>
            <tr>
              <td>Charcoal</td>
              <td>5-30 g</td>
              <td>1-3 g</td>
            </tr>
            <tr>
              <td>Peat</td>
              <td>50-100 g</td>
              <td>2 g</td>
            </tr>
            <tr>
              <td>Bones</td>
              <td>200-300 g</td>
              <td>1-3 g</td>
            </tr>
            <tr>
              <td>Organic sediments/soils</td>
              <td>500 g</td>
              <td>100 g</td>
            </tr>
          </tbody>
        </table>

        <h2 class="subtitle">
          ACCURACY OF THE CONVENTIONAL AGE DEPENDING ON THE SAMPLE AGE AND
          WEIGHT
        </h2>
        <div class="block">
          <table class="table">
            <thead>
              <tr>
                <th>Age</th>
                <th>Optimal mass of sample</th>
                <th>Minimal mass of sample</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>500 BP</td>
                <td>40 years</td>
                <td>60 years</td>
              </tr>
              <tr>
                <td>1000 BP</td>
                <td>50 years</td>
                <td>70 years</td>
              </tr>
              <tr>
                <td>5000 BP</td>
                <td>60 years</td>
                <td>90 years</td>
              </tr>
              <tr>
                <td>10000 BP</td>
                <td>70-90 years</td>
                <td>100-120 years</td>
              </tr>
              <tr>
                <td>20000 BP</td>
                <td>150-200 years</td>
                <td>250-300 years</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
  </div>

  <div class="container mt-6 o-kontakt" v-if="lindex !== 0">
    <div class="go-top" @click="goToBegin">^</div>
    <h1 class="title">Kontakt</h1>
    <div class="columns">
      <div class="column is-5">
        <div class="block lab-desc mt-6">
          <strong class="marg">Siedziba Laboratorium</strong><br />
          ul. Katowicka 17A<br />
          31-351 Kraków<br />
          <br />
          <strong class="marg">Dane kontaktowe</strong><br />
          tel.: +48 503 05 22 33<br />
          e-mail: laboratorium@c14.pl
        </div>
      </div>
      <div class="column">
        <map-component></map-component>
      </div>
    </div>
  </div>

  <div class="container mt-6 o-kontakt" v-if="lindex === 0">
    <div class="go-top" @click="goToBegin">^</div>
    <h1 class="title">Contact</h1>
    <div class="columns">
      <div class="column is-5">
        <div class="block lab-desc mt-6">
          <strong class="marg">Laboratory address:</strong><br />
          ul. Katowicka 17A<br />
          31-351 Kraków, Poland<br />
          <br />
          <strong class="marg">Contact</strong><br />
          phone.: +48 503 05 22 33<br />
          mail: laboratorium@c14.pl
        </div>
      </div>
      <div class="column">
        <map-component></map-component>
      </div>
    </div>
  </div>
</template>

<script>
import MapComponent from "./MapComponent.vue";

export default {
  components: {
    MapComponent,
  },
  props: ["lindex"],
  methods: {
    scrollToElem(elem) {
      const el = document.getElementsByClassName(elem)[0];
      if (el) {
        el.scrollIntoView({ behavior: "smooth" });
      }
    },
    goToBegin() {
      window.scrollTo({ top: 0, left: 0, behavior: "smooth" });
    },
  },
};
</script>

<style>
.title {
  padding-left: 1rem;
  color: #007dc6;
}

.navbar-item img {
  height: 100px !important;
  max-height: 100px !important;
  transform: translateY(-10px);
}
.subtitle {
  color: #007dc6;
  text-align: center;
  width: 100%;
  font-weight: bold;
}

.thead {
  font-weight: 900;
}
.block {
  text-align: justify;
  padding: 0 30px;
}

.block strong {
  color: #007dc6;
}

.marg {
  margin-left: 30px;
}

.under-line {
  border-bottom: 3px solid rgb(230, 230, 230);
  padding-bottom: 40px;
}
.under-line::after {
  content: "";
  width: 180px;
  display: block;
  border-bottom: 3px solid #007dc6;
  transform: translateY(43px);
  z-index: 11200;
}

.is-128x128 {
  margin: 10px;
}

.show-more {
  position: relative;
  background: #85a3b41a;
  padding: 30px;
  border: 1px solid rgb(216, 216, 216);
}

.important-text {
  color: #007dc6;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  position: absolute;
  top: 5px;
  right: 15px;
  font-weight: 700;
}

.table {
  margin: 0px auto;
  text-align: center;
}

th {
  color: white;
  background-color: rgb(230, 230, 230);
}

.qmenu {
  text-align: center;
}
.qmenu li {
  display: inline-block;
  padding: 10px 20px;
  font-weight: 700;
  cursor: pointer;
}

/* .qmenu li:not(:last-child) {
  border-right: 1px solid grey;
} */

.lab-desc {
  display: block;
  font-size: 15pt;
  text-align: justify;
  padding: 30px;
}

.go-top {
  position: absolute;
  display: inline;
  width: 30px;
  height: 30px;
  top: 10px;
  right: 20px;
  color: #007dc6;
  background-color: rgb(230, 230, 230);
  /* color: white; */
  font-weight: 700;
  font-size: 12pt;
  padding: 0px 7px;
  cursor: pointer;
}
</style>
