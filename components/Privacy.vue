<style>

    /* work-sans-regular - latin-ext_latin */
@font-face {
  font-family: 'Work Sans';
  font-style: normal;
  font-weight: 400;
  src: local(''),
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-regular.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-regular.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

/* work-sans-600 - latin-ext_latin */
@font-face {
  font-family: 'Work Sans';
  font-style: normal;
  font-weight: 600;
  src: local(''),
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-600.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-600.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

/* work-sans-800 - latin-ext_latin */
@font-face {
  font-family: 'Work Sans';
  font-style: normal;
  font-weight: 800;
  src: local(''),
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-800.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-800.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

/* work-sans-italic - latin-ext_latin */
@font-face {
  font-family: 'Work Sans';
  font-style: italic;
  font-weight: 400;
  src: local(''),
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-italic.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-italic.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

/* work-sans-600italic - latin-ext_latin */
@font-face {
  font-family: 'Work Sans';
  font-style: italic;
  font-weight: 600;
  src: local(''),
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-600italic.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-600italic.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

/* work-sans-800italic - latin-ext_latin */
@font-face {
  font-family: 'Work Sans';
  font-style: italic;
  font-weight: 800;
  src: local(''),
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-800italic.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
       url('~/assets/fonts/worksans/work-sans-v13-latin-ext_latin-800italic.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}
   .bg-a100c-1 {
      background: rgb(255,0,249);
      background: linear-gradient(90deg, rgba(255,0,249,0.25) 0%, rgba(255,117,0,0.25) 50%, rgba(255,0,35,0.25) 100%);
   }
   .bg-a100c-2 {
      background: rgb(255,0,249);
      background: linear-gradient(90deg, rgba(255,117,0,0.15) 0%, rgba(255,0,35,0.15) 50%, rgba(255,0,249,0.15) 100% );
   }
   .bg-a100c-3 {
      background: rgb(255,0,249);
      background: linear-gradient(90deg, rgba(255,0,35,0.15) 0%, rgba(255,0,249,0.15) 50%, rgba(255,117,0,0.15) 100% );
   }
   .bg-white {
    background-color: white;
   }
    button.text-link,
    a.text-link {
      text-decoration: none;
      background-image: linear-gradient(120deg, #fde68a 0, #fde68a 100%);
      background-repeat: no-repeat;
      background-size: 100% 0.4em;
      background-position: 0 100%;
    }
    h1 {
      @apply pb-0 pt-1 pl-5 pr-5 text-xl
    }
    h3, h4 {
      @apply pb-0 pt-4 pl-5 pr-5 font-semibold
    }
    p {
      @apply pb-2 pt-2 pl-5 pr-5
    }

  </style>

<template>
<div id="page">
  <div class="relative flex items-top justify-center min-h-screen bg-pink-100 bg-a100c-1 sm:items-center sm:pt-0">
    <div class="max-w-4xl mx-auto sm:px-6 lg:px-12">
      <div class="flex">
        <div class="flex align-center justify-center mt-8 pt-8 pl-10 sm:pt-0 mr-auto">
          <nuxt-link to="/">
            <img src="~/assets/a-thousand-channels--logo-variant-a--short.png" title="A thousand channels">
          </nuxt-link>
        </div>
        <div class="flex justify-right ml-auto mt-auto px-2">

        </div>
      </div>
      <div class="mt-8 bg-white overflow-hidden shadow sm:rounded-md p-6">
        <h1 class="leading-7">
          <nuxt-link to="/">
            A Thousand Channels –  {{ $t('project_part1') }} <img src="~/assets/lgbtq+_rainbow_flag_quasar_progress_flag_variant.svg" class="h-6 inline p-1" title="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black." alt="Pride flag variant based on Daniel Quasar's 2018 design combining elements of the Philadelphia flag and the trans pride flag, and brown and black."> {{ $t('project_part2') }}
          </nuxt-link>
        </h1>
      </div>
      <div class="mt-4 bg-white overflow-hidden shadow sm:rounded-md text-sm p-6">
        <h3 class="text-semibold">Datenschutz</h3>
        <p class="text-gray-800">
          Im Folgenden möchten wir Euch aufklären, wie Eure Daten von uns verarbeitet werden.
        </p>
        <p>
          Verantwortlich im Sinne der DSGVO ist:<br />
          Ulf Treger<br />
          Anschrift: Gaußstraße 25b, 22765 Hamburg<br />
          E-Mail: ut@a-thousand-channels.xyz
        </p>
        <p>
          Sollten Sie per E-Mail [oder über Kontaktformular] mit uns Kontakt aufnehmen, werden die mitgeteilten Daten von uns gespeichert, um Ihr Anliegen zu bearbeiten.
        </p>
        <p>
          Zu den verarbeiteten Daten zählen: Name, E-Mail-Adresse
        </p>
        <p>
          Wir werden die Daten löschen, sobald die Speicherung nicht mehr erforderlich ist oder die Verarbeitung einschränken, falls gesetzliche Aufbewahrungspflichten bestehen.
        </p>
      </div>
      <div class="mt-4 bg-white overflow-hidden shadow sm:rounded-md text-sm p-6 mb-4">
        <h3 class="text-semibold">Betroffenenrechte</h3>
        <p>
          Sie haben als betroffene Person, das Recht auf Auskunft, das Recht auf Berichtigung oder Löschung, das Recht auf Einschränkung der Verarbeitung und das Recht auf Widerspruch gegen die Verarbeitung Ihrer Daten. Sofern Sie uns eine Einwilligung erteilt haben, können Sie diese jederzeit mit Wirkung für die Zukunft widerrufen.
        </p>
        <p>
          Bitte richten Sie Ihren Widerspruch [oder Widerruf] formlos an folgende Adresse:
        </p>
        <p>
          Adresse siehe oben
        </p>
        <p>
          Darüber hinaus haben Sie das Recht auf Datenübertragbarkeit. Sie haben weiter das Recht, sich bei einer Aufsichtsbehörde über die Verarbeitung zu beschweren. Eine Liste der entsprechenden Behörden finden Sie unter: https://www.bfdi.bund.de/DE/Infothek/Anschriften_Links/anschriften_links-node.html.
        </p>
      </div>
      <div class="mt-2 bg-white overflow-hidden shadow sm:rounded-md text-sm p-6 mb-4">
        <h3 class="text-semibold">Hosting</h3>
        <p class="text-gray-800">
          Unser Hoster erhebt in sog. Logfiles folgende Daten, die Ihr Browser übermittelt:
        </p>
        <p>
          IP-Adresse, die Adresse der vorher besuchten Website (Referer Anfrage-Header), Datum und Uhrzeit der Anfrage, Zeitzonendifferenz zur Greenwich Mean Time, Inhalt der Anforderung, HTTP-Statuscode, übertragene Datenmenge, Website, von der die Anforderung kommt und Informationen zu Browser und Betriebssystem.
        </p>
        <p>
          Das ist erforderlich, um unsere Website anzuzeigen und die Stabilität und Sicherheit zu gewährleisten. Dies entspricht unserem berechtigten Interesse im Sinne des Art. 6 Abs. 1 S. 1 lit. f DSGVO.
        </p>
        <p>
          Es erfolgt kein Tracking und wir haben auf diese Daten keinen direkten Zugriff, sondern erhalten lediglich eine anonymisierte, statistische Zusammenfassung. Diese beinhaltet die Adresse der vorher besuchten Seite, die Häufigkeit der jeweils aufgerufenen Seiten und die Anzahl eindeutiger Besucher. Diese Daten führen wir nicht mit anderen Daten zusammen.
        </p>
        <p>
          Wir setzen für die Zurverfügungstellung unserer Website folgenden Hoster ein:
        </p>
        <p>
          GitHub Inc.<br />
          88 Colin P Kelly Jr St<br />
          San Francisco, CA 94107<br />
          United States<br />
        </p>
        <p>
          Dieser ist Empfänger Ihrer personenbezogenen Daten. Dies entspricht unserem berechtigten Interesse im Sinne des Art. 6 Abs. 1 S. 1 lit. f DSGVO, selbst keinen Server in unseren Räumlichkeiten vorhalten zu müssen. Serverstandort ist USA.
        </p>
        <p>
          Weitere Informationen zu Widerspruchs- und Beseitigungsmöglichkeiten gegenüber GitHub finden Sie unter: https://docs.github.com/en/free-pro-team@latest/github/site-policy/github-privacy-statement#github-pages
        </p>
        <p>
          Sie haben das Recht der Verarbeitung zu widersprechen. Ob der Widerspruch erfolgreich ist, ist im Rahmen einer Interessenabwägung zu ermitteln.
        </p>
        <p>
          Die Daten werden gelöscht, sobald der Zweck der Verarbeitung entfällt.
        </p>
        <p>
          Die Verarbeitung der unter diesem Abschnitt angegebenen Daten ist weder gesetzlich noch vertraglich vorgeschrieben. Die Funktionsfähigkeit der Website ist ohne die Verarbeitung nicht gewährleistet.
        </p>
        <p>
          GitHub hat Compliance-Maßnahmen für internationale Datenübermittlungen umgesetzt. Diese gelten für alle weltweiten Aktivitäten, bei denen GitHub personenbezogene Daten von natürlichen Personen in der EU verarbeitet. Diese Maßnahmen basieren auf den EU-Standardvertragsklauseln (SCCs). Weitere Informationen finden Sie unter: https://docs.github.com/en/free-pro-team@latest/github/site-policy/github-data-protection-addendum#attachment-1–the-standard-contractual-clauses-processors
        </p>
        <p class="text-sm">
          Diese Erklärung basiert auf <a href="https://opr.vc/docs/hosting/github_pages/#muster-datenschutzerkl%C3%A4rung">opr.vc</a> (CC0-Lizenz)
        </p>
      </div>
      <Footer></Footer>

    </div>
  </div>
</div>
</template>



<script>
export default {
 data() {
    return {

    }
  }
}
</script>