# Stand-alone Procfile buildpack in the Tiny builder

## Proposal

The Procfile buildpack should be added as a stand-alone group to the Tiny
builder's group orderings.

## Motivation

Adding the Procfile buildpack as a stand-alone order at the end of the group
ordering list would provide users that want to run pre-built binaries on the
smallest base image available a supported path to do so.

## Source Material

* The Procfile buildpack is alread a stand-alone buildpack in both the
  [Base](https://github.com/paketo-buildpacks/base-builder/blob/77f77454f74f6eb1d71c9b2d38eb9194350f66da/builder.toml#L80-L84)
  and the
  [Full](https://github.com/paketo-buildpacks/full-builder/blob/8069fea85dab14880f1dc54fcba552bb9fce3e70/builder.toml#L100-L104)
  builders.
* Te Procfile buildpack [supports the Tiny
  stack](https://github.com/paketo-buildpacks/procfile/blob/a36fb09721cd8fa05215333379e406e20391612f/buildpack.toml#L26-L27).
