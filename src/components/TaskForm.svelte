<script>
import PriorityButton from './PriorityButton'
</script>

<style>
.py-3 {
    padding-top: 1rem !important;
    padding-bottom: 1rem !important;
}
.small {
    font-size: 80%;
    font-weight: 400;
}
.text-white {
    color: #fff !important;
}
.form-control {
    display: block;
    width: 100%;
    padding: 0.5rem 0.75rem;
    font-size: 1rem;
    line-height: 1.25;
    color: #495057;
    background-color: #fff;
    background-image: none;
    background-clip: padding-box;
    border: 1px solid rgba(0,0,0,0.15);
    border-radius: 0.25rem;
    transition-property: border-color, box-shadow;
    transition-duration: 0.15s, 0.15s;
    transition-timing-function: ease-in-out, ease-in-out;
    transition-delay: 0s, 0s;
}
</style>

<form name="taskForm">
    <div class="container py-3">
        <div class="row">
            <div class="col-xl-5 mb-2 mb-xl-0">
                <div class="mb-1 small text-white">内容<span class="badge badge-danger ml-2">※必須</span></div>
            </div>
            <div>
                <input 
                    type="text"
                    name="content"
                    class="form-control"
                    requierd
                    placeholder="タスクを入力してください"
                >
            </div>
        </div>
        <div class="col-xl row">
            <div class="col-sm-auto col-md-auto col-xl">
                <div class="mb-1 small text-white">
                    優先度
                    <span class="badge badge-danger ml-2">※必須</span>
                </div>
                <PriorityButton/>
            </div>
            <div class="col-auto col-sm-auto col-xl mb-3 mb-sm-0"></div>
            <div class="col-sm-auto col-lg col-xl aligin-self-center"></div>
        </div>
    </div>
</form>