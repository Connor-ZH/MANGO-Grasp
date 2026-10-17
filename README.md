# MANGO-Grasp

**Mahalanobis Fields over Geometry-Oriented 3D Gaussians for Cross-Embodiment Dexterous Grasping**

Heng Zhang, Kevin Yuchen Ma, Mike Zheng Shou, Weisi Lin, and Yan Wu.

[Project page](https://connor-zh.github.io/MANGO-Grasp/) · [arXiv preprint](https://arxiv.org/abs/2608.02014) · [Video](https://www.youtube.com/watch?v=pAtVOlEqN5k)

MANGO-Grasp models hand–object interaction with anisotropic Mahalanobis fields over geometry-oriented 3D Gaussian primitives. Pretrained morpho-kinematic hand descriptors and a shared grasp optimization support cross-embodiment dexterous grasping, including zero-shot transfer to an unseen hand.

## Publication and release status

The paper is available as a 2026 arXiv preprint and has not yet been formally published. This repository currently contains the project website. The research code, data, and checkpoints will be released upon publication; the corresponding website controls remain disabled until those resources are available.

## Website files and local preview

- `index.html`: paper content, citation metadata, Open Graph, Twitter Card, and JSON-LD.
- `static/css/index.css`: project styles.
- `static/js/index.js`: page interactions.
- `static/images/method_overview.jpg`: the method figure.
- `static/videos/*.mp4`: ten real-world grasping demonstrations.

No build step is required. From the repository root, run:

```sh
python3 -m http.server 8000
```

Then open <http://localhost:8000/>.

## Metadata and deployment

The deployed URL is <https://connor-zh.github.io/MANGO-Grasp/>. It returned HTTP 200 with HTML identical to commit `60eacca19555d009423f0caf59ededcead2dcfb6` when checked on October 17, 2026; the arXiv abstract also links to this address. If the site moves, update the canonical URL, `og:url`, JSON-LD page URLs, and this README together.

Keep the visible title and authors, BibTeX, citation tags, social metadata, and JSON-LD consistent. The citation year is the preprint's year, 2026. `citation_online_date` records the verified arXiv posting date, August 3, 2026. Neither field asserts journal publication. JSON-LD intentionally omits a formal publication date, publisher, and paper license until those details are confirmed. Template attribution and website licensing below do not establish a license for the paper or unreleased research code.

No local paper PDF is committed, so no `citation_pdf_url` is advertised. The arXiv link remains the paper access point. If a local PDF is added later, verify its contents and public URL before adding the PDF metadata.

### Social sharing image

There is currently no dedicated share image. The broken `social_preview.png` references have been removed, and Twitter uses a `summary` card without an explicit thumbnail. Open Graph likewise has no explicit image; a platform may choose its own fallback.

To enable an explicit large-image preview:

1. Add an approved PNG or JPEG, for example a 1200 × 630 image, to `static/images/`.
2. Verify that its absolute URL under the deployed site returns an image successfully.
3. Add matching `og:image` and `twitter:image` tags, descriptive alt text, and the image's actual dimensions. Switch `twitter:card` to `summary_large_image`.
4. Check the deployed page in the intended sharing platforms; local HTML checks cannot verify their cached previews.

The existing method figure is 8572 × 3698 pixels and is retained as the full-resolution paper figure. It has not been repurposed as a social card. Twitter account tags remain omitted until real account handles are supplied.

## Citation

```bibtex
@misc{zhang2026mangograspmahalanobisfieldsgeometryoriented,
  title={MANGO-Grasp: Mahalanobis Fields over Geometry-Oriented 3D Gaussians for Cross-Embodiment Dexterous Grasping},
  author={Heng Zhang and Kevin Yuchen Ma and Mike Zheng Shou and Weisi Lin and Yan Wu},
  year={2026},
  eprint={2608.02014},
  archivePrefix={arXiv},
  primaryClass={cs.RO},
  url={https://arxiv.org/abs/2608.02014},
}
```

## Website attribution and license

This website uses the [Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template), adapted from [Nerfies](https://nerfies.github.io/).

The website template's existing [Creative Commons Attribution-ShareAlike 4.0 International license](https://creativecommons.org/licenses/by-sa/4.0/) is retained. Bundled third-party assets retain their own license notices.
