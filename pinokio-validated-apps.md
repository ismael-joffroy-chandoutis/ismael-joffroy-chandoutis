# Apps Pinokio validées — liste de confiance

> Liste curatée des apps Pinokio considérées fiables, soit parce qu'elles sont
> **vérifiées officiellement** par Cocktail Peanut (le créateur de Pinokio), soit
> parce qu'elles sont publiées par des **membres établis et actifs** de la communauté.
>
> **Dernière mise à jour : 2026-05-31** (passe automatique `/pinokio-update`)

---

## Le modèle de confiance Pinokio (à lire d'abord)

Pinokio distingue deux catégories de scripts :

- **Verified scripts** — explicitement relus, testés et approuvés par l'admin Pinokio
  (Cocktail Peanut). Ils vivent dans l'organisation GitHub **[pinokiofactory](https://github.com/pinokiofactory)**.
  Le repo doit être transféré à l'org (il est alors « gelé » sous contrôle de l'org),
  testé à la main, et validé sur des critères de sécurité (chemins isolés, venv isolé,
  paquets tiers confinés à `~/pinokio`, réputation du repo).
- **Community scripts** — listés automatiquement (repos GitHub taggés `pinokio`),
  **non approuvés**. Cocktail Peanut le dit explicitement :

  > « By default I do NOT recommend installing community scripts UNLESS you trust the
  > person who wrote the script. » — [@cocktailpeanut, juin 2025](https://x.com/cocktailpeanut/status/1932229427032621258)

**Règle d'or de cette liste :** une app n'entre ici que si elle est (1) dans
`pinokiofactory` (= vérifiée), **ou** (2) publiée par un acteur identifié, actif et
suivi de la communauté. Tout le reste = à vos risques, vérifiez le code.

---

## Acteurs fiables de la communauté

Les publishers qui reviennent le plus, actifs et avec un historique de scripts qui
fonctionnent. À suivre / sources de confiance pour découvrir de nouvelles apps.

| Publisher | Spécialité | Profil |
|---|---|---|
| **Cocktail Peanut** (`@cocktailpeanut`) | Créateur de Pinokio. Référence absolue. | [GitHub](https://github.com/cocktailpeanut) · [X](https://x.com/cocktailpeanut) |
| **Morpheus** (`@morpheus` / `6morpheus6`) | TTS, vidéo GPU-poor, voix — ~99 publications | [Profil Pinokio](https://beta.pinokio.co/u/morpheus) |
| **PierrunoYT** | TTS / voice cloning prolifique (DramaBox, OmniVoice, LuxTTS…) | [GitHub](https://github.com/PierrunoYT) |
| **mrbizarro** (`bizarro`) | Vidéo/image générative locale sur Apple Silicon | [Phosphene](https://beta.pinokio.co/apps/github-com-mrbizarro-phosphene) |
| **theinaog** | TTS low-VRAM (VoxCPM — synthèse multilingue tokenizer-free + voice cloning) | [beta.pinokio.co](https://beta.pinokio.co/) |
| **krynsky** | Outils média (ReClip — downloader vidéo/audio self-hosted, UI web) | [beta.pinokio.co](https://beta.pinokio.co/) |
| **IAnMove** | TTS multilingue low-VRAM (VoxCPM) | profil Pinokio |
| holandeb · gujjubhai · dimz · clawt · digifxron | Contributeurs récurrents vus en page d'accueil Pinokio | [beta.pinokio.co](https://beta.pinokio.co/) |
| _À vérifier_ : maoper · supersoniquestudio · itouch44 | Publishers vus récemment en vedette, à confirmer (activité/historique) | [beta.pinokio.co](https://beta.pinokio.co/) |

> Pour valider un nouvel acteur : présence sur le Discord Pinokio, historique de repos
> qui marchent, et idéalement des scripts repris dans `pinokiofactory`.

---

## ✅ Apps vérifiées officiellement (org `pinokiofactory`)

Les plus installées / étoilées de l'organisation vérifiée. (⭐ = stars GitHub au moment
de la maj.)

### Image
| App | Description | ⭐ |
|---|---|---|
| [flux-webui](https://github.com/pinokiofactory/flux-webui) | Web UI pour FLUX | 189 |
| [RMBG-2-Studio](https://github.com/pinokiofactory/RMBG-2-Studio) | Suppression/remplacement d'arrière-plan (BRIA-RMBG-2.0), low VRAM 6GB | 266 |
| [clarity-refiners-ui](https://github.com/pinokiofactory/clarity-refiners-ui) | Upscaler / enhancer créatif (Refiners), 8GB VRAM | 52 |
| [MFLUX-WEBUI](https://github.com/pinokiofactory/MFLUX-WEBUI) | Web UI MFLUX (Gradio + MLX, Apple Silicon) | 23 |
| [diffusers-image-fill](https://github.com/pinokiofactory/diffusers-image-fill) | Inpainting / fill | 21 |
| [invoke](https://github.com/pinokiofactory/invoke) · [omnigen](https://github.com/pinokiofactory/omnigen) · [instantir](https://github.com/pinokiofactory/instantir) | Suites image diverses | — |

### Vidéo
| App | Description | ⭐ |
|---|---|---|
| [cogstudio](https://github.com/pinokiofactory/cogstudio) | Studio vidéo CogVideo — l'app la plus étoilée de l'org | 392 |
| [wan](https://github.com/pinokiofactory/wan) | Wan video | 37 |
| [Frame-Pack](https://github.com/pinokiofactory/Frame-Pack) | Génération vidéo progressive (next-frame prediction) | 21 |
| [pyramidflow](https://github.com/pinokiofactory/pyramidflow) | PyramidFlow txt2vid | — |
| [Allegro-txt2vid-install](https://github.com/pinokiofactory/Allegro-txt2vid-install) | Allegro txt2vid (lent, 12GB+ VRAM) | — |
| [facepoke](https://github.com/pinokiofactory/facepoke) | Manipulation de visage | 18 |
| [hunyuanvideo](https://github.com/pinokiofactory/hunyuanvideo) | HunyuanVideo génération vidéo | 18 |
| [ai-video-composer](https://github.com/pinokiofactory/ai-video-composer) | Composition vidéo assistée par IA | 17 |
| [hallo](https://github.com/pinokiofactory/hallo) | Animation de portrait pilotée par l'audio | 13 |

### Audio / TTS / voix
| App | Description | ⭐ |
|---|---|---|
| [e2-f5-tts](https://github.com/pinokiofactory/e2-f5-tts) | E2 / F5 TTS | 80 |
| [Ultimate-TTS-Studio](https://github.com/pinokiofactory/Ultimate-TTS-Studio) | All-in-one : Kokoro, KittenTTS, Higgs, Chatterbox, Fish-Speech, F5, index-tts | 27 |
| [openaudio](https://github.com/pinokiofactory/openaudio) | OpenAudio | 27 |
| [Nari-Dia-TTS](https://github.com/pinokiofactory/Nari-Dia-TTS) | TTS basé Dia-1.6B (Nari Labs) | 34 |
| [Orpheus-TTS-FastAPI](https://github.com/pinokiofactory/Orpheus-TTS-FastAPI) | Orpheus TTS via FastAPI | 21 |
| [diffrhythm](https://github.com/pinokiofactory/diffrhythm) | DiffRhythm — génération musicale | 19 |
| [yue](https://github.com/pinokiofactory/yue) | YuE — génération de chansons (paroles + voix) | 18 |
| [StyleTTS2_Studio](https://github.com/pinokiofactory/StyleTTS2_Studio) | Crée ta propre voix StyleTTS 2 | 12 |
| [whisper-webui](https://github.com/pinokiofactory/whisper-webui) | Installer Whisper-WebUI (transcription/sous-titres) | 12 |
| [MMAudio](https://github.com/pinokiofactory/MMAudio) | Génération audio synchronisée à la vidéo | 12 |
| [mlx-video-transcription](https://github.com/pinokiofactory/mlx-video-transcription) | Transcription vidéo (MLX, Apple Silicon) | 13 |
| [zonos](https://github.com/pinokiofactory/zonos) · [dia](https://github.com/pinokiofactory/dia) | TTS additionnels | — |

### 3D
| App | Description | ⭐ |
|---|---|---|
| [Hunyuan3d-2-lowvram](https://github.com/pinokiofactory/Hunyuan3d-2-lowvram) | Hunyuan3D 2 en low VRAM | 22 |
| [TRELLIS](https://github.com/pinokiofactory/TRELLIS) | Génération 3D (Microsoft TRELLIS) | 18 |

### LLM / dev / divers
| App | Description | ⭐ |
|---|---|---|
| [bolt](https://github.com/pinokiofactory/bolt) | Bolt (dev assistant) | 59 |
| [comfy](https://github.com/pinokiofactory/comfy) | ComfyUI packagé | 26 |
| [openui](https://github.com/pinokiofactory/openui) | OpenUI — génère des interfaces depuis une description | 19 |
| [open-webui](https://github.com/pinokiofactory/open-webui) | Open WebUI — interface de chat LLM self-hosted | 18 |
| [macOS-use](https://github.com/pinokiofactory/macOS-use) | Rend les apps macOS accessibles aux agents IA | 13 |

> Catalogue complet : **[github.com/orgs/pinokiofactory/repositories](https://github.com/orgs/pinokiofactory/repositories?type=all&sort=stargazers)** (~100 repos vérifiés).

---

## 🟢 Apps communauté de confiance (publishers identifiés)

Non gelées dans `pinokiofactory`, mais publiées par des acteurs établis ci-dessus.

### Morpheus (`@morpheus`)
- **Wan2GP** — UI Gradio ultra-optimisée pour vidéo IA sur GPU « pauvres » (6GB+ VRAM) — [page](https://beta.pinokio.co/apps/github-com-6morpheus6-wan2gp)
- **Kokoro-TTS-Multilingual** — TTS multilingue rapide, 54 voix / 8 langues
- **IndexTTS-2** — TTS zero-shot expressif, contrôle de durée
- **Whisper-WebUI** — sous-titrage via Whisper
- **Forge Neo** — SD WebUI léger (Flux & Qwen, NVIDIA)
- **X-Voice / XVoice** — TTS 27 langues, un seul speaker
- **Kokoro-FastAPI** — wrapper API pour KokoroTTS (intègre Open-WebUI)
- **Sam3D** — meshes 3D de poses corporelles depuis des images
- **SongGeneration Studio** — génération de chansons avec contrôle de style (NVIDIA)

### PierrunoYT (TTS / voix)
- **[DramaBox-TTS](https://github.com/PierrunoYT/DramaBox-TTS-Pinokio)** — TTS expressif, voice cloning (LTX)
- **[OmniVoice](https://github.com/pierrunoyt/omnivoice-pinokio)** — TTS zero-shot 600+ langues, voice design
- **[LuxTTS](https://github.com/PierrunoYT/LuxTTS-Pinokio)** — voice cloning 48kHz, 150x+ realtime
- **[Soprano-TTS](https://github.com/PierrunoYT/soprano-tts-pinokio)**
- **[Pocket-TTS](https://github.com/PierrunoYT/pocket-tts-pinokio)** — TTS CPU-only, faible latence

### mrbizarro
- **[Phosphene](https://beta.pinokio.co/apps/github-com-mrbizarro-phosphene)** — vidéo/image générative locale + entraînement visage/voix in-app (Apple Silicon)

### theinaog (anc. attribué à IAnMove)
- **VoxCPM** — TTS multilingue tokenizer-free + voice cloning, faible VRAM

### krynsky
- **ReClip** — downloader vidéo/audio self-hosted open-source, UI web propre, multi-plateformes

### Cocktail Peanut (en page d'accueil, hors org)
- **Stable Audio 3** — launcher Stable Audio 3 (musique / SFX)
- **HiDream O1 Image FP8** — génération d'image (NVIDIA CUDA)
- **WorldMirror 2.0** — reconstruction 3D depuis HY-World 2.0 (NVIDIA, PyTorch + gsplat)
- **ds4-webui** — DeepSeek V4 Flash (Metal) · **Overworld** — générateur de monde temps réel

---

## Comment cette liste est maintenue

- **Source verité « vérifié » :** [org pinokiofactory](https://github.com/orgs/pinokiofactory/repositories?type=all&sort=stargazers) — tout ce qui y est = approuvé.
- **Source « communauté » :** [beta.pinokio.co](https://beta.pinokio.co/) (page d'accueil + profils `/u/<publisher>`) et le Discord Pinokio pour jauger l'activité.
- **Critère d'inclusion :** vérifié OU publisher identifié + actif + historique fiable.
- **Critère d'exclusion :** script anonyme / one-shot non audité → reste « community, à vos risques ».

### Pour mettre à jour — depuis n'importe quel appareil
Le repo embarque une **commande slash** : depuis Claude (web, mobile, desktop, CLI)
connecté à ce repo, tape simplement :

```
/pinokio-update
```

Elle exécute tout le playbook en autonomie (scan `pinokiofactory` trié par stars + profils
des acteurs fiables → édition du fichier → commit/push → PR avec résumé). Ajoute `--no-pr`
pour mettre à jour le fichier sans ouvrir de PR.

Le playbook complet vit dans [`.claude/commands/pinokio-update.md`](.claude/commands/pinokio-update.md).
Pour un rafraîchissement **planifié** (sans intervention), voir [`MAINTENANCE.md`](MAINTENANCE.md).

---

### Sources
- [pinokiocomputer/pinokio — README (modèle verified/community)](https://github.com/pinokiocomputer/pinokio/blob/main/README.md)
- [Org pinokiofactory (apps vérifiées)](https://github.com/orgs/pinokiofactory/repositories?type=all&sort=stargazers)
- [beta.pinokio.co (annuaire communauté)](https://beta.pinokio.co/)
- [Profil @morpheus](https://beta.pinokio.co/u/morpheus)
- [@cocktailpeanut sur la confiance des scripts communauté](https://x.com/cocktailpeanut/status/1932229427032621258)
