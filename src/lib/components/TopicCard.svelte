<div class="card lg:card-side bg-base-100 shadow-xl">
    <slot name="figure"></slot>
    <div class="card-body">
      <h2 class="card-title"><slot name="title"></slot></h2>
      <slot name="description"></slot>
      <div class="card-actions justify-end">
        <slot name="button"></slot>
      </div>
    </div>
  </div>