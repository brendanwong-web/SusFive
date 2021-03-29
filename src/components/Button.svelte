<style lang="scss" global>
    @import 'style/theme.scss';
    button {
        padding: 0.7rem 2rem;
        letter-spacing: 2.5px;
        border: 1px solid rgba(82, 182, 154, 0.452);
        background-color: white;
        color: $green-2;
        border-radius: 999px;
        font-size: 1.3rem;
        font-weight: 600;
        text-transform: capitalize;
        outline: none;
        box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.1);
        transition: all 0.1s ease-in;

        &:hover {
            color: $green-3;
            cursor: pointer;
            box-shadow: 0px 15px 20px #52b69a93;
            transform: translateY(-2px);
            transform: scale(1.05);
        }

    }
</style>

<button>
    <slot />
</button>