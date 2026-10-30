
# 3DGS for Interactive Visual Content: A Shared World for Film and Games

**Sumeru AI | Technical Perspective**

AI is changing how 3D content can be created. One promising direction is to move beyond generating a fixed sequence of frames and toward creating visual content that can be viewed, edited, and interacted with from different perspectives.

We believe 3D Gaussian Splatting (3DGS) could become one useful representation in this shift. It is not a replacement for every existing 3D format. Its potential lies in combining detailed appearance with real-time viewing and interaction.

## What makes 3DGS different?

Traditional 3D workflows often use polygon meshes. A mesh describes an object's surface using vertices, edges, and polygons, with materials and textures added to define its appearance. This makes meshes well suited to established workflows for topology, UV editing, collision, deformation, and animation.

3DGS represents a scene using many Gaussian primitives. Each primitive carries attributes such as position, color, opacity, scale, and orientation. Together, they can represent fine visual detail, including hair, fur, feathers, and vegetation.

These representations preserve different information and serve different needs:

| Consideration             | 3DGS                                                            | Polygon mesh                                                       |
| ------------------------- | --------------------------------------------------------------- | ------------------------------------------------------------------ |
| Primary strength          | Detailed appearance, including complex visual textures          | Explicit geometry and mature production workflows                  |
| Editing                   | Per-splat operations are possible; workflows are still evolving | Mature tools for topology, UVs, and materials                      |
| Animation and deformation | Depends on the representation and driving method                | Well established for rigging and deformation                       |
| Collision and physics     | Often requires additional geometry or processing                | Commonly supported by existing engine workflows                    |
| Best fit                  | High-fidelity visual content and selected scene types           | Gameplay objects, deformable characters, and geometry-driven tasks |

This is a simplified comparison. Performance and suitability depend on scene complexity, hardware, engine support, and implementation.

## From reconstructed scenes to generated content

One established use of 3DGS is reconstructing real environments from multi-view images or video. The result can be explored from different viewpoints instead of being limited to the original camera footage.

AI generation points toward a broader possibility: creating 3D assets and scenes that do not exist as complete captured references. This raises additional challenges, including consistency across viewpoints, editability, interaction, and integration into real-time applications.

For creators, the difference matters. A generated image or video is usually consumed as a fixed view. A 3D scene can let the camera move, the viewpoint change, and selected elements respond to the user.

## A shared 3D content pipeline for film and games

Imagine generating a set of 3D characters, environments, and props, then using them across multiple forms of content. The same scene could be rendered as a carefully composed video or used as the foundation for a real-time interactive experience.

This could support a more reusable production pipeline:

1. Generate or reconstruct 3D assets and scenes.
2. Arrange them in a shared environment.
3. Create or drive animation.
4. Design camera paths and interactions.
5. Render the result as video or deliver it as an interactive experience.

The same assets could be reused across shots, storylines, and interactive applications. This may reduce repeated asset creation, while giving creators more control over camera movement and scene continuity.

This is a direction for development, not a claim that every part of the pipeline is solved. Asset quality, animation, memory use, level of detail, and engine integration all need to be evaluated for the target project.

## What Sumeru AI is working on

Sumeru AI is developing tools for AI-powered 3D asset generation and dynamic content.

**Mugen3D** supports generating 3D assets from a single image, with 3DGS and mesh output options. The assets are intended for use in applications such as 3D presentation, digital content production, game development, and 3D printing.

**Mugen Morph** focuses on speech-driven lip motion and facial animation for 3D digital humans. We are also developing real-time full-body animation capabilities.

**TalkingHead** provides a workflow for creating conversational digital humans from a person's image and connecting them to dialogue applications.

These capabilities are under active development. Available features and output quality depend on the version and workflow being used.

## Conclusion

3DGS offers another way to represent visual content. It can preserve complex appearance and support free viewpoint exploration, while meshes remain important where explicit geometry, deformation, and mature editing workflows are required.

The opportunity is to choose the right representation for each part of a project—and, where useful, combine them. Over time, a shared set of AI-generated 3D assets could support both high-quality video and interactive experiences, helping bring film and games closer within the same content pipeline.

## References

- Kerbl et al., “3D Gaussian Splatting for Real-Time Radiance Field Rendering,” SIGGRAPH 2023.
- Mildenhall et al., “NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis,” ECCV 2020.
- World Labs, *Marble: A Multimodal World Model.*
- World Labs, *Atlas: A World Model for Spatial Intelligence.*
- Sumeru AI, *3D Generation & AI Avatar API.*

*This article presents Sumeru AI’s perspective. Product capabilities and development status are based on company materials and are not an independent third-party evaluation.*
