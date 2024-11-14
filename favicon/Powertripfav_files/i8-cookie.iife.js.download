this["i8-cookie"]=this["i8-cookie"]||{};this["i8-cookie"].js=function(){"use strict";const S="cookie",A="94e80c13abc08fc5900f727rzn3",k="i8cookie",_="https://icons8.com/privacy-policy",s={NECESSARY:"necessary",CUSTOMIZE:"customize",DETAILS:"details",SWITCH:"switch",SAVE:"save",ALL:"all"},l={NECESSARY:"necessary",FUNCTIONAL:"functional",PERFORMANCE:"performance",MARKETING:"marketing"},d={[l.NECESSARY]:!0,[l.FUNCTIONAL]:!1,[l.PERFORMANCE]:!1,[l.MARKETING]:!1},N=Object.fromEntries(Object.entries(d).map(([e])=>[e,!0])),O={en:"en-US",zh:"zh-CN",fr:"fr-FR",de:"de-DE",it:"it-IT",ja:"ja-JP",pt:"pt-BR",ru:"ru-RU",es:"es-ES",ko:"ko-KR"};function R(e,t={}){return{title:e("COOKIE_MAIN.TITLE"),whatFor:e("COOKIE_MAIN.WHAT_FOR"),detailsTitle:e("COOKIE_MAIN.DETAILS_TITLE"),linkTitle:e("COOKIE_MAIN.LINK_TITLE"),link:t.cookiePolicy||_,customizeTitle:e("COOKIE_MAIN.CUSTOMIZE_TITLE"),customizeDescription:e("COOKIE_MAIN.CUSTOMIZE_DESCRIPTION"),buttons:{btnAll:e("COOKIE_BUTTONS.BTN_ALL"),btnNecessary:e("COOKIE_BUTTONS.BTN_NECESSARY"),btnCustomize:e("COOKIE_BUTTONS.BTN_CUSTOMIZE"),btnSave:e("COOKIE_BUTTONS.BTN_SAVE")},categories:[{key:l.NECESSARY,title:e("COOKIE_CATEGORIES.NECESSARY.TITLE"),description:e("COOKIE_CATEGORIES.NECESSARY.DESCRIPTION"),activeText:e("COOKIE_CATEGORIES.NECESSARY.ACTIVE_TEXT")},{key:l.FUNCTIONAL,title:e("COOKIE_CATEGORIES.FUNCTIONAL.TITLE"),description:e("COOKIE_CATEGORIES.FUNCTIONAL.DESCRIPTION")},{key:l.PERFORMANCE,title:e("COOKIE_CATEGORIES.PERFORMANCE.TITLE"),description:e("COOKIE_CATEGORIES.PERFORMANCE.DESCRIPTION")},{key:l.MARKETING,title:e("COOKIE_CATEGORIES.MARKETING.TITLE"),description:e("COOKIE_CATEGORIES.MARKETING.DESCRIPTION")}]}}function v(e){return`
    <div class="i8-cookie-popup__buttons">
      <button class="i8-cookie-button i8-cookie-button--light" data-cc="${s.ALL}">
        ${e.btnAll}
      </button>

      <button class="i8-cookie-button" data-cc="${s.NECESSARY}">
        ${e.btnNecessary}
      </button>

      <button class="i8-cookie-button i8-cookie-button--customize" data-cc="${s.CUSTOMIZE}">
        ${e.btnCustomize}
      </button>

      <button class="i8-cookie-button i8-cookie-button--save" data-cc="${s.SAVE}">
        ${e.btnSave}
      </button>
    </div>
  `}function f(e){return`
    <label class="i8-cookie-switch">
      <input 
        type="checkbox"
        value="${e.key}"
        data-cc="${s.SWITCH}"
        ${e.checked?"checked":""}
      />
      <span></span>
    </label>
  `}function p(e){const t=e.activeText?`<div class="i8-cookie-category__active">${e.activeText}</div>`:f({key:e.key,checked:e.checked});return`
    <div class="i8-cookie-category">
      <div class="i8-cookie-category__head">
        <div class="i8-cookie-category__title">
          ${e.title}
        </div>
        ${t}
      </div>
      <div class="i8-cookie-category__description">
        ${e.description}
      </div>
    </div>
  `}function L(e){return`
    <div class="i8-cookie-popup" role="dialog">
      <div class="i8-cookie-popup__logo"></div>
      <div class="i8-cookie-popup__content">
        <div class="i8-cookie-popup__default">
          <div class="i8-cookie-popup__title">
            ${e.title} <a data-cc="${s.DETAILS}">${e.whatFor}</a>
          </div>
        </div>

        <div class="i8-cookie-popup__details">
          <div class="i8-cookie-popup__title">${e.detailsTitle}</div>
          <a href="${e.link}" target="_blank">${e.linkTitle}</a>
        </div>

        <div class="i8-cookie-popup__customize">
          <div class="i8-cookie-popup__title">
            ${e.customizeTitle}
          </div>
          <div>
            ${e.customizeDescription}
          </div>
        </div>

        <div class="i8-cookie-popup__categories i8-cookie-scroll">
          ${e.categories.map(p).join("")}
        </div>

        ${v(e.buttons)}
      </div>
    </div>
  `}function T(e,t){document.dispatchEvent(new CustomEvent(e,{detail:t}))}function m(e={}){let t=null;const E={...d},i=(n,I)=>{const r=t==null?void 0:t.querySelectorAll(`[data-cc="${n}"]`);r==null||r.forEach(u=>{u instanceof HTMLElement&&(u.onclick=I)})},a=()=>{i(s.DETAILS,()=>{t==null||t.classList.add("i8-cookie--details")}),i(s.CUSTOMIZE,()=>{t==null||t.classList.add("i8-cookie--customize")}),i(s.NECESSARY,()=>T("cc:accept",d)),i(s.ALL,()=>T("cc:accept",N)),i(s.SAVE,()=>T("cc:accept",E)),i(s.SWITCH,({target:n})=>{n instanceof HTMLInputElement&&(E[n.value]=n.checked)})};return{render:n=>{t||(t=document.createElement("div"),t.className="i8-cookie",t.style.zIndex=String(e.zIndex||100),t.innerHTML=L(n),document.body.appendChild(t),a())},destroy:()=>{t==null||t.remove(),t=null,Object.assign(E,d)}}}function b(e={}){const t={loading:!1};return{fetchTranslates:async()=>{if(t.translations||t.loading)return;t.loading=!0;const a=e.locale&&O[e.locale]||e.locale||O.en,c=`https://distributions.crowdin.net/${A}/content/${S}/${a}.json`;try{const o=await fetch(c);t.translations=await o.json()}catch{console.warn("Failed to receive translations.")}t.loading=!1},$t:a=>t.translations?a.split(".").reduce((c,o)=>typeof c=="object"&&o in c?c[o]:a,t.translations):a}}function y(e){const t=document.cookie.split("; ");for(const E of t){const[i,a]=E.split("=");if(i===e)return decodeURIComponent(a)}}function g(e={}){const t=e.storageName||k,E=e.storageExpiresDays||365,i=c=>{const o=c.timestamp||new Date().getTime(),n=JSON.stringify({timestamp:o,version:1,...c}),I=`${t}=${encodeURIComponent(n)};`,r=new Date(o);r.setDate(r.getDate()+E);const u=`expires=${r.toUTCString()};`;document.cookie=I+u+"path=/;"};return{setData:i,getData:()=>{const c=y(t);if(c)try{const o=JSON.parse(c);if(o.version===1)return i(o),o}catch{}}}}function C(e={}){const t=b(e),E=g(e),i=m(e),a=async()=>{E.getData()||await c()},c=async()=>{await t.fetchTranslates();const n=R(t.$t,e);i.render(n)},o=()=>{i.destroy()};return document.addEventListener("cc:accept",n=>{n instanceof CustomEvent&&E.setData(n.detail),i.destroy()}),{init:a,open:c,close:o}}return typeof window<"u"&&(window.I8Cookie=C,window.I8CookieReady&&window.I8CookieReady()),C}();
