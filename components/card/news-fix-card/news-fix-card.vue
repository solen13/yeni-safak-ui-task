<template>
  <div class="news-fix-card">
    <div class="news-fix-card__head">
      <span class="news-fix-card__head--categori"
        >Dünya
        <hr
      /></span>
      <button>
        <Icon name="heroicons:ellipsis-horizontal" size="22" />
      </button>
    </div>
    <div class="news-fix-card__image-content">
      <img
        class="news-fix-card__image-content--image"
        src="https://s3-alpha-sig.figma.com/img/7b57/9f70/e3c0c0dd8ab60a0e16fdd3097441c246?Expires=1718582400&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=SkT6axqmH4XnL7Q~DUBw1hYuKJ9c6ulyfUg3~tSdPCFeE5XbI5gSVf~HtWOxslODJ1fLtkqVoDwEdQYbIroYYfrx8ncbhNs7IVykGFoVPPkaA5JBSmsqUKKbSAcPbRWCeFq0OaA-xh5lA8Kt5N~41jW9qXgjNOG7iRZdhQbsXRh5ThDdVm6u4Rv~ZOh~HEjL8XkC2EcQfw4sg4Db3OYym-93yKa5ZskDrpZoIRnhFNp1lvwqVuxZkb2-uJDnJyn-bNNWp4VAxsb--sJJWaaVMBHEuq-hms-Tkg8UKfjisQGjj5w2g8h~epTQFRrk2TWIFpmlSV2rnQ~tAcIXkh91xw__"
        alt=""
      />
    </div>
    <div class="news-fix-card__button-content">
      <span class="news-fix-card__button-content--left">
        <button>
          <Icon name="mdi:cards-heart-outline" size="22" />
        </button>
        <button>
          <Icon name="iconamoon:comment" size="22" />
        </button>
      </span>
      <span class="news-fix-card__button-content--right">
        <button>
          <Icon name="streamline:mail-send-email-message" size="22" />
        </button>
        <button>
          <Icon name="game-icons:save-arrow" size="22" />
        </button>
      </span>
    </div>
    <div class="news-fix-card__comment-list">
      <img
        class="news-fix-card__comment-list--image"
        src="https://s3-alpha-sig.figma.com/img/b377/5cea/a7a7ed548e51795c7def3e04e8d3cddf?Expires=1718582400&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=bOpA3qpl~qD~o4uK5U3rKEw6mOT6lTa6c4~iOgWnWRKnIiRIPwPhza445x0BJbFBKgsq72eV8UlejcDO3palzj7-6rgTeFSDMkIRPE-PnxJnwPMC1vgrG8umNbdNrFQWlNPweZuZT9R0kODOEFGcojOYFy6ECmHycnMgzrEXSemIF8KBTY1DklTV2N51LzIo88MlZLkh0~z6DeXCKi8yNn-OnOvcaA0pzfhzL9JS1bPrjGJfSMRwCtSycW7Iiw7T3xfrJW3hkXr~FvuBCyavo4ZjPeA~KqQeYWZ2cht4xoOyAE1t2epPCjfzSVZSjBQT1nQrn3oq0tGJTaDxlG-N-g__"
        alt=""
      />
      <img
        class="news-fix-card__comment-list--image"
        src="https://s3-alpha-sig.figma.com/img/117c/3a57/fdc160483c372691f6cb7e5505f73634?Expires=1718582400&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=iSeJhLOg5o6iLJKXNQHndYGBCmI5pkzYIRV9ZOrRYf1xEBQnXwFeMe0L8pnTuskCzJAcE20zBcTu3FcBp0Ltli7qGfUJOov0ht6Vs1xWnu-Rpg0YD6iRygmilAlMK-hEu3SqljSb45bzaXMm545tJiceVXvuNyI7gEq7WTphlIVhmvUmU-6S76Fh1D2ZAW3HjH63oPiW-W~IKayb57CPayoplKjArFe-60AKsQJK-tHgA00MEkYNZT4hDtn~ICup7g6qVxr5lrGjGqA7t9B9sQZHIiFVHcnQ3bgArz-soEUschbpeLx3I8jXcgjr2NSaMjaF-pm5QlhtxOhtx9wkDg__"
        alt=""
      />
      Ömer Karaca ve 323 kişi beğendi, 5 yorum yazıldı.
    </div>
    <div class="news-fix-card__text">
      <h2 class="news-fix-card__text--title">
        ABD, Suudi Arabistan'a Patriot ve asker gönderecek
      </h2>
      <p class="news-fix-card__text-des">
        Apple tarafından bahar aylarında tanıtılması hedeflenen AirPower, ekstra
        bir sürprizle karşımıza çıkabilir. İddialara göre ikinci nesil AirPods
        da Air-Power ile aynı anda tanıtılacak. Hatta, AirPods 2’nin siyah renk
        seçeneği ile sunulması da söz konusu…
      </p>
    </div>

    <div class="px-4 my-3">
      <news-fix-comments-card />
    </div>

    <div class="news-fix-card__all-button">
      <button>
        <Icon
          name="material-symbols-light:radio-button-unchecked"
          size="10"
          color="#8D8D8D"
        />Tüm yorumları gör (27)
      </button>
    </div>
    <div class="news-fix-card__comment-write">
      <img
        class="news-fix-card__comment-write--profile"
        src="https://s3-alpha-sig.figma.com/img/7bf9/eee1/93cb0239b614c48ab5251817664cef35?Expires=1718582400&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=G2s4TlRHdyrtP0gseHUspR9UrKR5-3EJtoCk89Cnb7HCkd~lordh7kKfJCHuEsbERlCRmgCv6JgpzZZkhD5Ll6KHRQF9wFj-Lo4RL0NsKITtvx00ScRLD5tuwhoQZe-VCvnq6-ZlceRu3KwqQaxV0lQ50qz8x8zIGe-g2S~UCEzrH4yiGYGd6pbgz3F-229Wt4DPCo51toIxbKSzCCOZ-RQ98PfemSKL~K4y6d-GdirgnhSKCn8p9UcuImF8czuJP~To~LtBH0Nsaswp4skqXrDiTI1amPAPNhwbw63PiXdVk8aNUgGdDH00m2fZxQBX9E5Q6SIZLXZjF5lfEQ0HAQ__"
        alt=""
      />
      <input
        class="news-fix-card__comment-write--input"
        type="text"
        placeholder="Yorumunuzu ekleyin ..."
      />
      <button class="news-fix-card__comment-write--send-button">Gönder</button>
    </div>
  </div>
</template>
<style lang="scss" src="./news-fix-card.scss"></style>
