<!-- PLUGINLABS-ADVANCED-VARSAYILAN -->
## Varsayılan tasarım sistemi: PluginLabs Advanced

- Bu projede her arayüz, ekran, komponent, popup, panel, HTML/CSS veya stil işinde `pluginlabs-advanced` skill'i kullanılır. Eski temel `pluginlabs-design` skill'inin yerine geçer; temel katman (PLC-001…079) Advanced'in içinde aynen durur.
- Skill konumu: repoda `.claude/skills/pluginlabs-advanced/` varsa o, yoksa kişisel `~/.claude/skills/pluginlabs-advanced/`. Kanonik kaynak: `PluginLabs/design-system/pluginlabs-advanced/`.
- İşe başlamadan önce `SKILL.md` ve `references/TASARIM-PRENSIPLERI.md` okunur; komponent seçimi `references/KOMPONENTLER.md` üzerinden yapılır.
- CSS sırası: `assets/pl-tokens.css` → `assets/pl-components.css` → `assets/pl-advanced.css`. Kapsayıcı: `<div data-pl data-pl-theme="dark" data-pl-product="…">`.
- Ürünün mevcut `data-pl-product` aksanı korunur; yüzey gerekiyorsa `data-pl-surface="glass|hud|neon|soft|cockpit"`.
- Tam ekranlarda önce Ekran Şablonları (PLA-091…102) ve `assets/pl-pin-ekranlari.html` içindeki en yakın ekran temel alınır.
- Yalnız `[data-pl]` kapsayıcısı, `--pl-` tokenları ve `pl-` sınıfları; global seçici ve sabit renk yazılmaz.
- Mevcut tasarıma dokunulmaz: bir ekranı Advanced'e taşımak opt-in'dir, önce kullanıcıya sorulur. Silme yok, eskiler `_arsiv/GG.AA.YYYY/` altına taşınır.
- Claude Design karşılığı: "PluginLabs Advanced" tasarım sistemi — https://claude.ai/artifact/J9knwk3VLaYFpVC4u22cxC
<!-- /PLUGINLABS-ADVANCED-VARSAYILAN -->

## Workspace organization notes

- This folder is one independent Git checkout; do not treat other folders with the same origin as redundant without comparing their branches and work.
- Check `git status`, branch, and upstream before cleanup. Preserve user edits and untracked `_arsiv/` content; do not reset, clean, or delete work as part of organization.
- For any consolidation, compare commits and files first and ask before destructive moves or deletion.
- Commit only the intended documentation/code files, leaving unrelated pre-existing changes untouched.
- In the local `C:\Users\pc\github` workspace, use `PROJECT-ORGANIZATION.md` as the checkout inventory and verify its status before acting.
